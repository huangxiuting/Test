<template>
  <div id="app">
    <keep-alive>
      <router-view/>             <!--显示的就是HelloWorld.vue 这个组件里面的内容，通过路由地址展示-->
    </keep-alive>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style></style>
