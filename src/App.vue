<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
      <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
    </li>
    <Hello
     :msg="msg"
     :msg2="'hhhhhh'"
     @chikButtonClick="increase"
    />
    <button @click="increase">{{ count }}</button>
  </div>
</template>

<script>
import Hello from './components/Hello.vue'
export default {
  name: 'App',
  components: {
    Hello
  },
  data () {
    return {
      todos: [
        { id: 1, text: 'hoge' },
        { id: 2, text: 'hooo' }
      ],
      msg: 'msgHello',
      count: 0
    }
  },
  methods: {
    increase () {
      this.count = this.count + 1
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
