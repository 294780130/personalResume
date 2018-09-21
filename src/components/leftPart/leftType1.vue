<template>
  <div class="left1">
    <div v-for="item in info" class="line">
      <div class="picture">
        <img src="static/images/1.png" v-if="item.img==1">
        <img src="static/images/2.png" v-else-if="item.img==2">
        <img src="static/images/3.png" v-else-if="item.img==3">
        <img src="static/images/4.png" v-else>
      </div>
      <div class="context"><span>{{item.context}}</span></div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    info: {
      type: Array,
      required: true
    }
  },
  data () {
    return {
      data() {
        return {

        }
      },
      mounted () {
      },
    }
  }
}
</script>

<style scoped>
.left1{
  margin-bottom: 55px;
}
.line{
  display: flex;
  margin-bottom: 12px;
}
.picture{
  width: 28px;
  height: 28px;
  background-color: #fff;
  border-radius: 8px;
  margin-left: 26px;
  /* flex-basis: 54px; */
}
.picture img{
  width: 20px;
  height: 20px;
  margin: 4px;
}
.context{
  flex:1;
  margin-left:16px; 
  line-height: 28px;
}
span{
  flex: 1;
  color: #8897a2;
  background-image: url('');
}
</style>

