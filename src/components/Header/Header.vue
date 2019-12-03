<template>
  <div class="header">
    <van-nav-bar left-arrow :border="false" class="top">
      <van-dropdown-menu slot="right" class="right">
        <van-dropdown-item title="三亚" />
      </van-dropdown-menu>
      <van-search placeholder="请输入搜索关键词" slot="title" />
    </van-nav-bar>
  </div>
</template>

<script>
export default {}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl';

.header {
  height: 43px;

  .top {
    display: flex;
    align-items: center;
    background-color: $bgColor;

    .right {
      height: 43px;
      color: #ccc;
      background-color: $bgColor;
    }
  }
}

.van-search {
  padding: 0;
}

.van-hairline--top-bottom::after {
  border: none !important;
}

.van-nav-bar__right {
  bottom: auto;
}
</style>