<template>
  <div class="left2">
    <div class="title">{{title}}</div>
    <div v-for="item in info" class="item">
      <div class="topic">{{item.topic}}</div>
      <div v-for="(lab,index) in sum" v-if='index<item.count' class="par">
        <v-parallelogram :color="item.color" :empty=false></v-parallelogram>
      </div>
      <div v-for="(lab,index) in sum" v-if='index<(sum-item.count)' class="par">
        <v-parallelogram :color="item.color" :empty=true></v-parallelogram>
      </div>
    </div>
  </div>
</template>

<script>
import parallelogram from './parallelogram.vue'
export default {
  props: {
    info: {
      type: Array,
      required: true
    },
    title: {
      type: String,
      required:true
    },
    sum: {
      type: Number,
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
  },
  components: {
    'v-parallelogram': parallelogram
  }
}
</script>

<style scoped>
.left2{
  color: #8897a2;
  line-height: 28px;
  padding-left: 26px;
  margin-bottom: 55px;
}
.item{
  margin-top: 10px;
  height: 28px;
  font-size: 0;
}
.topic{
  width: 94px;
  display: inline-block;
  font-size: 16px;
}
.par{
  display: inline;
}
</style>

