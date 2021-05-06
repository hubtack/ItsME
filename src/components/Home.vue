<template>

  <div class="nav">
    <HeadTab />
<!--    <div>-->
<!--      <ul class="tabStyle">-->
<!--        <li v-for="(item,index) in topTab" :key="index">-->
<!--          <span>{{item.lable}}</span>-->
<!--        </li>-->
<!--      </ul>-->
<!--    </div>-->
    <div class="content">
      <div>
        <div class="introduce">It's ME</div>
        <div class="name">lonely people</div>
      </div>
      <div class="date">
        {{nowYear}}
      </div>
      
    </div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>
    <div>22</div>



  </div>
</template>


<script>
import HeadTab from './HeadTab.vue'
export default {
  name:"Home",
  components:{HeadTab},
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
      ],
      nowYear:''
    }
  },

  mounted(){
    let nowDate = new Date()
    this.nowYear = nowDate.getFullYear()
  },
  methods:{


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
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-left: 10%;
  margin-right: 3%;
  margin-top: 10%;
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

  .date{
    font-family:"HELVEYI1";
    font-size: 35px;
  }


  .img{
    display : block ;
    opacity: 0.2;

  }
}

  }


</style>