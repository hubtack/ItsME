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
  }
}
</script>

<style lang="less">

#app {
  width: 100%;
  height: 100%;
  position: fixed;
  background-image: linear-gradient(0deg, #ffffff, #98C6A6);
  background-size: 100% 100%;
  animation: blinds 4s ease-in-out infinite alternate;
  color: transparent;
  z-index: -1;
  color: #000000;

  #circle{
    position: absolute;
    border-radius: 50%;
    animation: circles 15s linear infinite alternate;
    z-index: -1;
  }
}

@keyframes blinds {

  0% {
    background-image:linear-gradient(45 deg, #ffffff, #98c6a6);
  }
  50% {
    background-image:linear-gradient(90 deg, #ffffff, #98C6A6);
  }
  100% {
    background-image:linear-gradient(260 deg, #ffffff, #98C6A6);
  }
}
@keyframes circles {
  0%,100% {
    top: 20px;
    right:20px;
    width: 150px;
    height: 150px;
    background-image: radial-gradient(rgba(133, 134, 186,0.8), transparent);
    filter: blur(20px);
  }

  50% {
    top: 100px;
    right:100px;
    width: 300px;
    height: 300px;
    background-image: radial-gradient(rgba(133, 134, 186,0.8), transparent);
    filter: blur(80px);
  }
}
</style>
