<template>
  <div class="rightTitle">
    <!-- <h3 class="txt" :style="{'background-color':color}">{{title}}<span class="triangle" :style="{'border-top-color':color}"></span></h3> -->
    <h3>{{title}}</h3>
    <span class="line" :style="{'background-color':color}"></span>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    color: {
      type: String,
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
        // alert(this.$refs.myInfo.msg)
        console.log(this.title)
      },
    }
  }
}
</script>

<style scoped>
.rightTitle{
  display: flex;
}
.rightTitle h3 {
    margin: 0;
    margin-top: 10px;
    display: inline-block;
    font-size: 23px;
    color: black;
    padding-right: 10px;
}
.rightTitle .line {
    display: inline-block;
    flex: 1;
    height: 10px;
    position: relative;
    top: 20px;
}
</style>

