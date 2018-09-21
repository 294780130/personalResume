<template>
  <div class="par">
      <div class="parallelogram" :style="{'background-color':color, 'border-color':color}" v-if="!empty"></div>
      <div class="parallelogram" :style="{'border-color':color}" v-else></div>
  </div>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      required:true
    },
    empty: {
      type: Boolean,
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
par{
  font-size: 0;
}
.parallelogram{
    margin-right: 5px;
    display: inline-block;
    padding: 5px 12px;
    color: #333;
    transform: skew(-20deg);
    border: 1px solid #000;
}
</style>

