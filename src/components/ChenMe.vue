<template>
  <div>
    <button @click="switchClick">点击切换</button>
  </div>
</template>

<script>
export default {
  name: "ChenMe",
  data() {
    return {
      msGetStats: "世界和平"
    }
  },
  props: {
    msg: String
  },
  methods:{
    switchClick(){
      this.$emit('switchShow')
    }
  }
}
</script>

<style scoped>
.color {
  color: blue;
}
</style>