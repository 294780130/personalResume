<template>
  <div class="left4">
    <div class="picture" v-for="item in info">
      <img :src="item" />
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
  },
  components: {
    
  }
}
</script>

<style scoped>
.left4{
  display: flex;
}
.picture{
  width: 33%;
  flex: 1;
  text-align: center;
}
.left4 img{
  width:80%;
}
</style>

