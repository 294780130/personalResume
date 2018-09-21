<template>
  <div class="right5">
    <div class="line" v-for="item in info.text">
      <u></u><p>{{item}}</p>
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
.right5{
  color: #808085;
  font-size: 15px;
}
p{
  margin: 0;
  display: inline;
}
u{
  display: inline-block;
  width: 8px;
  height: 8px;
  border-radius: 4px;
  background-color: #808085;
  margin-right: 8px;
}
.line{
  line-height: 26px;
}
</style>

