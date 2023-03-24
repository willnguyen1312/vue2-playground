<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <CoolButton />
  </div>
</template>

<script>
// @ is an alias to /src
import CoolButton from "@/components/CoolButton.vue";

export default {
  name: "HomeView",
  components: {
    CoolButton,
  },
};
</script>
