<template>

  <div class="nav">
    <div>
      <ul class="tabStyle">
        <li v-for="(item,index) in topTab" :key="index">
          <span>{{item.lable}}</span>
        </li>
      </ul>
    </div>
    <div class="content">
      <div class="introduce">It's ME</div>
      <div class="name">lonely people</div>
<!--      <div class="name">people</div>-->
    </div>

  </div>
</template>


<script>
export default {
  name:"Home",
  data(){
    return {
      topTab:[{
        lable:'HOME',
      },{
        lable:'HE',
      },{
        lable:'THIS',
      },{
        lable:'ABOUT',
      },
      ]
    }

  }

}





</script>


<style scoped lang="less" >

.nav{
.tabStyle{
  display: flex;
  li{
    margin-right: 10px;
    width: 100px;
  }
}

.content{
  margin-left: 10%;
  margin-top: 25%;
  .introduce{
    font-family:"HELVEYI1";
    font-size: 100px;
    font-style: italic;
    line-height: 0.5;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale
  }
  .name{
    font-family:"SJ";
    font-size: 70px;
    font-style: italic;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale
  }
}

  }


</style>