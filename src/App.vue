<template>
  <div id="app">
    <!-- <img src="./assets/logo.png">
    <router-view/> -->
    <!-- 数据存储 -->
    <v-info ref='myInfo'></v-info>
    <div class="paper">
      <div class="left">
        <div v-for="(item,key) in leftPart">
          <v-leftTitle :title="item.text" :color="item.color"></v-leftTitle>
          <v-left1 v-if="item.type==1" :info="item.info"></v-left1>
          <v-left2 v-else-if="item.type==2" :info="item.info" :title="item.title" :sum="item.sum"></v-left2>
          <v-left3 v-else-if="item.type==3" :info="item.info" :sum="item.sum"></v-left3>
          <v-left4 v-else-if="item.type==4" :info="item.info"></v-left4>
        </div>
        <v-leftBottom></v-leftBottom>
      </div>
      <div class="right">
        <h1>郑浩琦 Zheng Haoqi</h1>
        <h2>求职意向/前端开发工程师</h2>
        <div v-for="(item,key) in rightPart">
          <v-rightTitle :title="item.text" :color="item.color"></v-rightTitle>
          <div v-for="(part,num) in item.context">
            <v-right1 v-if="part.type==1" :info="part"></v-right1>
            <v-right2 v-else-if="part.type==2" :info="part"></v-right2>
            <v-right3 v-else-if="part.type==3" :info="part"></v-right3>
            <v-right4 v-else-if="part.type==4" :info="part"></v-right4>
            <v-right5 v-else-if="part.type==5" :info="part"></v-right5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Info from './components/Info.vue'
import leftPartTitle from './components/leftPart/leftTitle'
import leftType1 from './components/leftPart/leftType1'
import leftType2 from './components/leftPart/leftType2'
import leftType3 from './components/leftPart/leftType3'
import leftType4 from './components/leftPart/leftType4'
import leftBottom from './components/leftPart/leftBottom'
import rightPartTitle from './components/rightPart/rightTitle'
import rightType1 from './components/rightPart/rightType1'
import rightType2 from './components/rightPart/rightType2'
import rightType3 from './components/rightPart/rightType3'
import rightType4 from './components/rightPart/rightType4'
import rightType5 from './components/rightPart/rightType5'
export default {
  data () {
    return {
      leftPart: [],
      rightPart: []
    }
  },
  mounted () {
    this.leftPart = this.$refs.myInfo.leftPart
    this.rightPart = this.$refs.myInfo.rightPart
  },
  methods: {

  },
  components: {
    'v-info': Info,
    'v-leftTitle': leftPartTitle,
    'v-left1': leftType1,
    'v-left2': leftType2,
    'v-left3': leftType3,
    'v-left4': leftType4,
    'v-leftBottom': leftBottom,
    'v-rightTitle': rightPartTitle,
    'v-right1': rightType1,
    'v-right2': rightType2,
    'v-right3': rightType3,
    'v-right4': rightType4,
    'v-right5': rightType5
  }
}
</script>

<style>
#app .paper{
  width: 960px;
  height: 1350px;
  background-color: white;
  margin: 20px auto;
  box-shadow: 0 2px 6px rgba(100, 100, 100, 0.3);
}
#app .left{
  width: 275px;
  height: 1234px;
  background-color: #07426C;
  float: left;
  padding: 86px 15px 30px 30px;
}
#app .right{
  width: 560px;
  height: 1275px;
  float: left;
  padding: 75px 40px 0 40px;
}
#app .right h1 {
    color: black;
    font-size: 40px;
    margin-top: 0px;
    margin-bottom: 12px;
}
#app .right h2 {
    margin: 0;
    font-size: 16px;
    color: black;
    font-weight: normal;
}
</style>
