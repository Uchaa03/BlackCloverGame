<template>
  <header-component/>
  <main class="container my-5">
    <SectionComponent/>
    <Section2Component/>
    <SectionVideoComponent/>
  </main>
  <FooterComponent/>
</template>

<script >
  import {defineComponent} from "vue";
  import SectionComponent from "@/components/SectionComponent.vue";
  import HeaderComponent from "@/components/HeaderComponent.vue";
  import Section2Component from "@/components/Section2Component.vue";
  import SectionVideoComponent from "@/components/SectionVideoComponent.vue";
  import FooterComponent from "@/components/FooterComponent.vue";

  export default defineComponent({
    components: {FooterComponent, SectionVideoComponent, Section2Component, HeaderComponent, SectionComponent}
  })
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

  :root {
    --font-family-pixel: 'Press Start 2P';
  }

  h1 {
    font-family: var(--font-family-pixel),serif;
  }
</style>

