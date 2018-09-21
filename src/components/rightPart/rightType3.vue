<template>
  <div class="right3">
    <u class="round"></u>
    <div v-for="item in info.text">{{item}}</div>
  </div>
</template>

<script>
export default {
  props: {
    info: {
      type: Object,
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
.right3{
  display: flex;
  color: #fda85c;
  font-size: 15px;

}
.right3 div{
  line-height: 20px;
  margin: 8px 30px 8px 0;
}
.round{
  display: block;
  width: 16px;
  height: 16px;
  border-radius: 8px;
  background-color: #fda85c;
  float: left;
  position: relative;
  top: 2px;
  margin: 8px 20px 0 0;
}
</style>

