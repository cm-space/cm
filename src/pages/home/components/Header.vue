<template>
  <div class="header">
    <span class="header-left">左</span>
    <label class="header-input">
      <input  class="header-input-one" placeholder="请求搜索">
    </label>

    <span class="header-right">右</span>
  </div>
</template>

<script>
export default {
  name: 'HeaderContent',
  data () {
    return {
      msg: 'header'
    }
  }
}
</script>

<style scoped>
.header {
  background: #25a4bb;
  display: flex;
}

.header-left {
  width: 40px;
  line-height: 40px;
  text-align: center;
  float: left;
}

.header-right {
  line-height: 40px;
  width: 40px;
  text-align: center;
  float: right;
}

.header-input {
  align-self: center;
  flex: 1;
}
.header-input-one {
  width: 100%;
  height: 30px;
}

</style>
