<template>
  <div class="left3">
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
.left3{
  color: #8897a2;
  margin-bottom: 60px;
}
.item{
  font-size: 0;
  padding-left: 26px;
  margin-bottom: 15px;
}
.topic{
  font-size: 16px;
  line-height: 21px;
  margin-bottom: 14px;
}
.par{
  display: inline;
}
</style>

