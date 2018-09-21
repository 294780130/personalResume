<template>
  <div class="leftBottom">
    <h4>PERSONAL</h4>
    <small>RESUME 个人简历</small>
    <div class="arrow">
        <div class="part1"></div>
        <div class="part2"></div>
        <div class="part3"></div>
        <div class="part4"></div>
    </div>
  </div>
</template>

<script>
export default {
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
.leftBottom{
  margin-top: 76px;
  color: #8897a2;
}
h4{
  font-weight: normal;
  font-size: 24px;
  margin: 0;
}
.arrow {
  position: relative;
  top: -14px;
  left: 115px;
}
.part1 {
  width: 20px;
  height: 10px;
  position: relative;
  background-color: #909a9c;
}
.part2 {
    width: 10px;
    height: 10px;
    border-radius: 0 0 100% 0;
    background-color: #909a9c;
    position: relative;
    left: 20px;
    top: -10px;
}
.part3 {
    width: 10px;
    height: 18px;
    background-color: #909a9c;
    position: relative;
    left: 20px;
    top: -38px;
} 
.part4 {
    width: 0;
    height: 0;
    border-left: 13px solid transparent;
    border-right: 13px solid transparent;
    border-bottom: 18px solid #909a9c;
    position: relative;
    left: 12px;
    top: -74px;
}
</style>

