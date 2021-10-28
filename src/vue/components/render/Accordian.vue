<template>
  <div class="w-full px-4 pt-16">
    <div class="w-full p-2 mx-auto bg-white rounded-2xl">
      <Disclosure v-slot="{ open }">
        <DisclosureButton
          class="
            flex
            justify-between
            w-full
            px-4
            py-2
            text-sm
            font-medium
            text-left text-purple-900
            bg-purple-100
            rounded-lg
            hover:bg-purple-200
            focus:outline-none
            focus-visible:ring
            focus-visible:ring-purple-500
            focus-visible:ring-opacity-75
          "
        >
          <span>Tech Specs</span>
          <ChevronUpIcon
            :class="open ? 'transform rotate-180' : ''"
            class="w-5 h-5 text-purple-500"
          />
        </DisclosureButton>
        <DisclosurePanel class="px-4 pt-4 pb-2 text-sm text-gray-500">
          <div
            class="
              flex flex-wrap
              -mx-1
              overflow-hidden
              sm:-mx-2
              lg:-mx-3
              xl:-mx-4
            "
          >
            <div
              class="
                grid grid-cols-3
                my-1
                px-1
                w-full
                mx-2
                overflow-hidden
                sm:my-2 sm:px-2 sm:w-full
              "
            >
              <!-- Column Content -->

              <div class="bg-blue-300">
                <div
                  class="
                    pb-2
                    mb-5
                    font-sans
                    text-xl
                    not-italic
                    font-light
                    leading-none
                    text-black
                    capitalize
                  "
                  style="text-transform: capitalize"
                >
                  Bulb 1
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>

                  <div class="">
                    <span
                      class="
                        block
                        text-base
                        font-light
                        leading-6
                        text-gray-900
                        box-border
                      "
                    >
                      1500 lumens (100W equivalent)
                    </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>

                  <div class="">
                    <span
                      class="
                        block
                        text-base
                        font-light
                        leading-6
                        text-gray-900
                        box-border
                      "
                    >
                      123ABC
                    </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span
                      class="
                        block
                        text-base
                        font-light
                        leading-6
                        text-gray-900
                        box-border
                      "
                    >
                      1500 lumens (100W equivalent)
                    </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div class="">
                    <span
                      class="
                        block
                        text-base
                        font-light
                        leading-6
                        text-gray-900
                        box-border
                      "
                    >
                      123ABC
                    </span>
                  </div>
                </div>
              </div>

              <!-- repeat -->

              <div
                class="
                  my-1
                  px-1
                  w-full
                  overflow-hidden
                  sm:my-2 sm:px-2 sm:w-full
                  md:w-1/2
                  lg:my-2 lg:px-2 lg:w-1/3
                  xl:my-5 xl:px-5 xl:w-1/3
                "
              >
                <!-- Column Content -->
                <div
                  class="
                    mx-2
                    pb-2
                    mb-5
                    font-sans
                    text-xl
                    not-italic
                    font-light
                    leading-none
                    text-black
                    capitalize
                    b
                  "
                  style="text-transform: capitalize"
                >
                  Bulb 2
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>
              </div>

              <div
                class="
                  my-1
                  px-1
                  w-full
                  overflow-hidden
                  sm:my-2 sm:px-2 sm:w-full
                  md:w-1/2
                  lg:my-2 lg:px-2 lg:w-1/3
                  xl:my-5 xl:px-5 xl:w-1/3
                "
              >
                <!-- Column Content -->

                <div class="mx-2 mt-3 uppercase font-extrabold">Bulb 3</div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>
              </div>

              <div
                class="
                  my-1
                  px-1
                  w-full
                  overflow-hidden
                  sm:my-2 sm:px-2 sm:w-full
                  md:w-1/2
                  lg:my-2 lg:px-2 lg:w-1/3
                  xl:my-5 xl:px-5 xl:w-1/3
                "
              >
                <!-- Column Content -->
                <div
                  class="
                    pb-2
                    mb-5
                    font-sans
                    text-xl
                    not-italic
                    font-light
                    leading-none
                    text-black
                    capitalize
                    border-b border-gray-300 border-solid
                    box-border
                  "
                  style="text-transform: capitalize"
                >
                  Bulb 4
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>
              </div>

              <div
                class="
                  my-1
                  px-1
                  w-full
                  overflow-hidden
                  sm:my-2 sm:px-2 sm:w-full
                  md:w-1/2
                  lg:my-2 lg:px-2 lg:w-1/3
                  xl:my-5 xl:px-5 xl:w-1/3
                "
              >
                <!-- Column Content -->
                <div
                  class="
                    pb-2
                    mb-5
                    font-sans
                    text-xl
                    not-italic
                    font-light
                    leading-none
                    text-black
                    capitalize
                    border-b border-gray-300 border-solid
                    box-border
                  "
                  style="text-transform: capitalize"
                >
                  Bulb 5
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>
              </div>

              <div
                class="
                  my-1
                  px-1
                  w-full
                  overflow-hidden
                  sm:my-2 sm:px-2 sm:w-full
                  md:w-1/2
                  lg:my-2 lg:px-2 lg:w-1/3
                  xl:my-5 xl:px-5 xl:w-1/3
                "
              >
                <!-- Column Content -->
                <div class="mt-3 uppercase font-extrabold">Bulb 6</div>
                xxx
                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Brightness </span></div>
                  <div class="">
                    <span class=""> 1500 lumens (100W equivalent) </span>
                  </div>
                </div>

                <div class="mt-4">
                  <div><span class="font-bold"> Model: </span></div>
                  <div><span class=""> 123ABC </span></div>
                </div>
              </div>

              <!-- end -->
            </div>
          </div>
        </DisclosurePanel>
      </Disclosure>
      <Disclosure as="div" class="mt-2" v-slot="{ open }">
        <DisclosureButton
          class="
            flex
            justify-between
            w-full
            px-4
            py-2
            text-sm
            font-medium
            text-left text-purple-900
            bg-purple-100
            rounded-lg
            hover:bg-purple-200
            focus:outline-none
            focus-visible:ring
            focus-visible:ring-purple-500
            focus-visible:ring-opacity-75
          "
        >
          <span>FAQ</span>
          <ChevronUpIcon
            :class="open ? 'transform rotate-180' : ''"
            class="w-5 h-5 text-purple-500"
          />
        </DisclosureButton>
        <DisclosurePanel class="px-4 pt-4 pb-2 text-sm text-gray-500">
          No.
        </DisclosurePanel>
      </Disclosure>
      <Disclosure as="div" class="mt-2" v-slot="{ open }">
        <DisclosureButton
          class="
            flex
            justify-between
            w-full
            px-4
            py-2
            text-sm
            font-medium
            text-left text-purple-900
            bg-purple-100
            rounded-lg
            hover:bg-purple-200
            focus:outline-none
            focus-visible:ring
            focus-visible:ring-purple-500
            focus-visible:ring-opacity-75
          "
        >
          <span>Product Reviews</span>
          <ChevronUpIcon
            :class="open ? 'transform rotate-180' : ''"
            class="w-5 h-5 text-purple-500"
          />
        </DisclosureButton>
        <DisclosurePanel class="px-4 pt-4 pb-2 text-sm text-gray-500">
          No.
        </DisclosurePanel>
      </Disclosure>
    </div>
  </div>
</template>

<script>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
import { ChevronUpIcon } from "@heroicons/vue/solid";

export default {
  components: {
    Disclosure,
    DisclosureButton,
    DisclosurePanel,
    ChevronUpIcon,
  },
};
</script>
