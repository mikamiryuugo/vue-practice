<template>
  <div>
    {{text}}
    <p>{{ msg }}</p>
    <p>{{ msg2 }}</p>
    <button @click="helloIncrease">increase!!!</button>
  </div>
</template>
<script>
export default {
  props: ['msg', 'msg2'],
  data () {
    return {
      text: 'helloTest'
    }
  },
  methods: {
    helloIncrease () {
      this.$emit('chikButtonClick')
    }
  }
}
</script>
<style lang="scss" scoped>

</style>
