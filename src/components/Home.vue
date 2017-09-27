<template>
  <div class="home">
    <md-toolbar>
      <md-button class="md-icon-button" @click="toggleLeftSidenav">
        <md-icon>menu</md-icon>
      </md-button>

      <h2 class="md-title" style="flex: 1">CNode Zone</h2>

      <md-button class="md-icon-button">
        <md-icon>favorite</md-icon>
      </md-button>
    </md-toolbar>
    
    <side-nav ref="sidenav"></side-nav>

  </div>
</template>


<script type="text/javascript">
import SideNav from './SideNav'
export default {
  name: 'home',
  methods: {
    toggleLeftSidenav () {
      this.$refs.sidenav.$refs.leftSidenav.toggle()
    }
  },
  components: {
    SideNav
  }
}
</script>