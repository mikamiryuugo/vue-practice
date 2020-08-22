<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
      <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
    </li>
  </div>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      todos: [
        { id: 1, text: 'hoge' },
        { id: 2, text: 'hooo' }
      ]
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
