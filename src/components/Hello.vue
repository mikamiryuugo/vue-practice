<template>
  <div>
    {{text}}
    <p>{{ msg }}</p>
    <p>{{ msg2 }}</p>
  </div>
</template>
<script>
export default {
  props: ['msg', 'msg2'],
  data () {
    return {
      text: 'helloTest'
    }
  }
}
</script>
<style lang="scss" scoped>

</style>
