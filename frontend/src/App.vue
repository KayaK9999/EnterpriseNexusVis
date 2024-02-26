<template>
  <div class="container">
    <header class="header">
      标题 + 基本设置
    </header>
    <div class="content">
      <div class="left">
        <!-- 基础信息栏 -->
        <BasicInformation />
      </div>
      <div class="middle">
        <div class="middle-top">散点图</div>
        <div class="middle-bottom">平行坐标图</div>
      </div>
      <div class="right">时序差分图</div>
    </div>
  </div>
</template>

<script>
import BasicInformation from './components/BasicInformation.vue';

export default {
  name: 'App',
  components: {
    BasicInformation,
  },
};
</script>

<style scoped>
/* 让元素的内边距和边框成为元素宽度和高度的一部分，而不是在宽度和高度之外添加 */
* {
  box-sizing: border-box;
}
.container {
  display: grid;
  grid-template-rows: 1fr 19fr;
  height: 98vh;
}

.header {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: brown;
  color: white;
  border: 2px solid red;
  margin: 2px;
}

.content {
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
}

.left,
.right {
  border: 2px solid green;
  margin: 2px;
  height: 100%;
}

.middle {
  display: grid;
  grid-template-rows: 3fr 2fr;
}

.middle-top,
.middle-bottom {
  border: 2px solid blue;
  margin: 2px;
}</style>