<template>
  <view class="content">
    <view class="name">照片墙</view>
    <view class="main">
      <view class="main-1">
        <view class="main-1-header">记忆</view>
        <view class="main-1-content">
          <view class="main-1-content-1">1</view>
          <view class="main-1-content-1">2</view>
          <view class="main-1-content-1">3</view>
          <view class="main-1-content-1">4</view>
        </view>
      </view>
      <view class="cc">
        <view class="main-2">
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
          <view class="main-2-content">
            <view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view>
          </view>
        </view>
        <view class="main-3">
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view></view
          >
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2"
              ><p>名字</p>
              <p>123</p></view
            ></view
          >
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view></view
          >
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view></view
          >
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view></view
          >
          <view class="main-3-content"
            ><view class="main-2-content-cc1">图片</view>
            <view class="main-2-content-cc2">名字</view></view
          >
        </view>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
};
</script>

<style >
.content {
}
.content .name {
  text-align: center;
}
.main-1-header {
  text-align: center;
}
.main-1-content {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 10px;
}

.main-1-content-1:nth-child(2n) {
  background: red;
}
.main-1-content-1:nth-child(2n-1) {
  background: yellow;
}
.main-1-content-1:nth-child(1) {
  grid-column: 1 / 3;
  grid-row: 1/3;
  width: 45vw;
  height: 45vw;
}
.main-1-content-1:nth-child(2) {
  grid-column: 3 / 5;
}
.main-1 {
  padding: 10px;
  box-sizing: border-box;
}
.main-1-header {
  margin-bottom: 10px;
}
.cc {
  display: flex;
}
.cc > view {
  flex: 1;
}
/* .main-3-content:nth-child(2n) {
  background: pink;
}
.main-3-content:nth-child(2n-1) {
  background: greenyellow;
} */
.main-2 {
  margin-right: 15px;
}
/* 单个内容 */
.main-2-content,
.main-3-content {
  margin-bottom: 10px;
}
.main-2-content-cc1 {
  width: 45vw;
  height: 45vw;
  background: green;
}
.cc {
  padding: 10px;
  box-sizing: border-box;
}
</style>
