<template>
  <button @click="increment">
    Count is: {{ count }}
  </button>
</template>

<script>
export default {
  name: 'CountDemo',
  // data 返回的属性将成为响应式的状态
  // 并且暴露在 this 上
  data() {
    return {
      count: 0
    }
  },

  // method 是一些用来更改状态与触发更新的函数
  // 可以在模版中作为事件监听器绑定
  methods: {
    increment() {
      this.count++
    }
  },

  // 生命周期钩子会在组件生命周期的各个不同的阶段被调用
  // 例如这个函数就会在组件挂载完成后被调用
  mounted() {
    console.log(`The initial count is ${this.count}.`)
  }
}
</script>

<style scoped>
button {
  font-weight: bold;
}
</style>