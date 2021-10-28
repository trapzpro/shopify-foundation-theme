<template>
  <div>
    <button @click="increment">increment</button>
    <button @click="decrement">decrement</button>
    <p>{{ count }}</p>
  </div>
</template>
<script>
export default {
  name: "Counter",
   props: {
    products: {
      type: Object,
      required: true
    }
  },
  data() {
    return { count: 0 };
  },
  methods: {
    increment() {
      this.count++;
    },
     howMany() {
       return this.products.count;
    },
    decrement() {
      this.count--;
    },
  },
};
</script>
