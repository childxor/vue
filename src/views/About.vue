<template>
  <div id="app2" class="about">
    <img alt="Vue logo" src="../assets/logo.png" />
  </div>
</template>

<script>
import { Component, Vue } from "vue-property-decorator";
import abc from "@/components/About.vue"; // @ is an alias to /src

@Component({
  components: {
    abc,
  },
})
export default class About extends Vue {}
</script>
