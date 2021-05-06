<template>
  <div class="nav">
    <div class="title">
      <div class="info">
        <div>
          Net.BinJ
        </div>
        <div>
          An elegant Coding youth
        </div>
      </div>
      <div>
        02 &nbsp;&nbsp;&nbsp;&nbsp; 1996
      </div>
    </div>
  </div>


</template>


<script>

export default {
  name:'HeadTab',
  data(){
    return{

    }
  },

}

</script>
<style scoped lang="less">

.nav{
  margin: 10px 35px;
  padding: 5px;
  border-bottom: 2px solid #000000;
  font-family: 'HELVEYI1';
  font-size: 20px;
  .title{
    display: flex;
    justify-content: space-between;
    .info{
      display: flex;
      justify-content: space-between;
      width: 35%;
    }
  }
}


</style>