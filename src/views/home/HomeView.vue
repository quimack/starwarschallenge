<template>
  <div class="wrapper">
    <HelloWorld msg="Star Wars"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style scoped lang="scss" src="./styles.scss"></style>

