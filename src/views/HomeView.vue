<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <CoolButton />
  </div>
</template>

<script>
// @ts-check

/**
 * @typedef {object} Item
 * @property {string} text
 */

import CoolButton from "@/components/CoolButton.vue";

export default {
  name: "HomeView",
  components: {
    CoolButton,
  },
  data() {
    return {
      /** @type Array<Item> */
      items: [],
    };
  },
  methods: {
    /** @param {number} input */
    sayHi(input) {
      this.items = [{ text: input.toString() }];
    },
  },
};
</script>
