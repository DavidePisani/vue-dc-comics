<template>
  <div id="app">

    <PageHeader/>
    
  
    <main>
      <JumboTron/>
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
import JumboTron from './components/JumboTron.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    MainSection,
    MainContent,
    EndPage,
    JumboTron,

  }
}
</script>

<style lang="scss">
 @import './style/common';

</style>
