<template>
  <!--瀑布流-->
  <div class="waterfall-container">
    <div class="waterfall-item" v-for="i in 100"> vue的语法，不会就粘贴20个div看效果
      内容... 这里可以自己实现宽高不一样的div，看效果
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang='less' rel="stylesheet/less" >
  .waterfall-container {
    /*分几列*/
    column-count: 2;
    /*列间距，可有可无，默认30px*/
    /*column-gap: 0;*/
    -moz-column-gap:40px; /* Firefox */
    -webkit-column-gap:40px; /* Safari 和 Chrome */
    column-gap:40px;
  }

  .waterfall-item {
    /*不留白，不知道什么意思可以取消这个样式试试*/
    break-inside: avoid;
  }
</style>
