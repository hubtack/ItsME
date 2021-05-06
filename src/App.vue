<template>
  <div id="app">
    <div id="circle">
    </div>
    <Home />
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home,
  },
  created() {

  },
  // beforeDestroy () {
  //   document.removeEventListener("scroll", this.listenerFunction);
  // },
  mounted(){
    let nowDate = new Date()
    this.nowYear = nowDate.getFullYear()
    this.listenerFunction();
  },
  methods:{
    listenerFunction() {
      document.addEventListener('scroll', this.handleScroll, true);
    },
    handleScroll () {
      // this.scroll = document.body.scrollTop;
      console.log(document.body.scrollTop)
      // console.log(window.pageYOffset)
    }

  }
}
</script>

<style lang="less">


</style>
