<template>
  <div class="right1">
    <div class="type1">
      <div class="title"><b></b>{{info.title}}</div>
      <div class="text">{{info.text[0]}}</div>
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
.type1{
  display: flex;
  color: #808085;
  font-size: 15px;
}
.text{
  flex: 1;
}
</style>

