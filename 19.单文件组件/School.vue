<template>
  <!-- 组件标签 -->
  <div class="demo">
    <h2>学校名称：{{ schoolName }}</h2>
    <h2>学校地址：{{ address }}</h2>
    <button @click="showName">点我提示学校名</button>
  </div>
</template>

<script>
// 组件交互相关
export default {
  name: "School",
  data() {
    return {
      schoolName: "尚硅谷",
      address: "北京",
    };
  },
  methods: {
    showName() {
      alert(this.schoolName);
    },
  },
};
</script>

<style>
/* 组件样式 */
.demo {
  background-color: orange;
}
</style>