<template>
  <div class="right4">
    <table>
      <tr v-for="item in info.text">
        <td>{{item.time}}</td>
        <td>{{item.department}}</td>
        <td>{{item.position}}</td>
      </tr>
    </table>
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
.right4 table{
  color: #808085;
  font-size: 15px;
  margin-top: 10px;
}

td{
  text-align: center;
  padding: 0 16px;
  height: 22px;
  line-height: 22px;
}
</style>

