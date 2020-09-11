<template>
  <div>
    <slot></slot>
    <h1 class="color">{{msg}}</h1>
  </div>
</template>

<script>
export default {
  name: "ChenMe",
  props: {
    msg:String
  }
}
</script>

<style scoped>
.color {
  color: blue;
}
</style>