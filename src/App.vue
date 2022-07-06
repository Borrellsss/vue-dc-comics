<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent/>

    <!-- MAIN -->
    <main>
      <!-- first section -->
      <MainFirstSection/>
      <!-- second section -->
      <MainSecondSection/>
    </main>

    <!-- FOOTER -->
    <FooterComponent/>
  </div>
</template>

<script>
// *IMPORTS
import HeaderComponent from './components/HeaderComponent.vue';
import MainFirstSection from './components/MainFirstSection.vue';
import MainSecondSection from './components/MainSecondSection.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainFirstSection,
    MainSecondSection,
    FooterComponent
  }
}
</script>

<style lang="scss">
// *IMPORTS
@import "./style/Variables.scss";
@import "./style/Common.scss";
</style>
