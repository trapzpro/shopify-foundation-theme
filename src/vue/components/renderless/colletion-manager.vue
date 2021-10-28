<script>
import { ref, toRef } from "vue";
const axios = require("axios");

export default {
  props: {
    products: {
      type: Object,
      required: true,
      default: null,
    },
  },
  setup(props, { slots }) {
    const products = toRef(props, "products");

    const loadMetafields = () => {
      products.value.forEach((item) => {
        console.log(item);
        axios
          .get("/products/" + item.handle + "?view=specs")
          .then(function (response) {
            // handle success
            var span = document.createElement("span");
            span.innerHTML = response.data;
            var innerjson = (span.textContent || span.innerText)
              .trim()
              .replace("=>", ":");
            console.log(innerjson);
            var jsonmeta = JSON.parse(innerjson);
            console.log(jsonmeta);

            //Find index of specific object using findIndex method.
            let objIndex = products.value.findIndex((obj) => obj.id == item.id);

            //Log object to Console.
            console.log("Before update: ", products.value[objIndex]);

            //Update object's name property.
            products.value[objIndex].metafields = { specs: jsonmeta };

            //Log object to console again.
            console.log("After update: ", products.value[objIndex]);
          })
          .catch(function (error) {
            // handle error
            console.log(error);
          })
          .then(function () {
            alert("Done");
          });
      });
      /*
       */
      products.value.forEach((item) => {
        console.log(item);
      });
    };

    return () =>
      slots.default({
        products: products.value,
        loadMetafields,
      });
  },
};
</script>
