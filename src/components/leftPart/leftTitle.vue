<template>
  <div class="leftTitle">
    <h3 class="txt" :style="{'background-color':color}">{{title}}<span class="triangle" :style="{'border-top-color':color}"></span></h3>
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
.txt{
  width: 244px;
  height: 36px;
  padding-left: 32px;
  line-height: 36px;
  font-size: 21px;
  color: white;
  margin-top: 0;
  margin-bottom: 38px;
}
.triangle{
  display: block;
  width: 0;
  height: 0;
  border-left: 8px solid transparent;
  border-right: 8px solid transparent;
  border-top: 16px solid transparent;
  position: relative;
  top: 0;
  left: 0;
}
</style>

