<template>
  <div id="app">

    <PageHeader/>
  
    <main>
      <MainSection/>
      <MainContent/>
    </main>

   <EndPage/>
  </div>
</template>

<script>

import PageHeader from './components/PageHeader.vue'
import MainSection from './components/MainSection.vue'
import MainContent from './components/MainContent.vue'
import EndPage from './components/EndPage.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    MainSection,
    MainContent,
    EndPage,

  }
}
</script>

<style lang="scss">
 @import './style/common';

</style>
