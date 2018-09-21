<template>
  <div class="right2">
    <div class="type2">
      <div class="title"><b></b>{{info.title}}</div>
      <div class="text" v-for="item in info.text"><b class="bg-white"></b>{{item}}</div>
    </div>
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
b{
  display: inline-block;
  width: 8px;
  height: 8px;
  background-color: #808085;
  position: relative;
  top: -2px;
  margin-right: 4px;
}
.text{
  padding-left: 34px;
}
.bg-white{
  background-color: #fff;
  border: 1px solid #808085;
}
.type2{
  color: #808085;
  font-size: 15px;
}

</style>

