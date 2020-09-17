<!--
 * @Author: your name
 * @Date: 2020-09-17 14:56:38
 * @LastEditTime: 2020-09-17 15:06:19
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /vueThreeDemo/src/components/HelloWorld.vue
-->
<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p v-for="item in ds" :key="item">
    Edit <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      count: 0,
      ds: [0, 1, 23, 4, 5, 6, 6, 6, 6, 7],
    };
  },
};
</script>
