<template>
  <div class="mdl-layout__container">
    <div class="demo-layout mdl-layout mdl-js-layout mdl-layout--fixed-drawer mdl-layout--fixed-header">
      <searchbar></searchbar>
      <sidebar></sidebar>
      <main class="mdl-layout__content mdl-color--grey-100">
        <div class="mdl-grid demo-content">
          <router-view></router-view>
        </div>
      </main>
    </div>
  </div>
</template>

<style>
</style>

<script type="text/babel">
  import Sidebar from './components/Sidebar.vue'
  import Searchbar from './components/Searchbar.vue'

  export default {
    data () {
      return {
        msg: 'hello vue'
      }
    },
    components: {
      Sidebar,
      Searchbar
    }
  }
</script>
