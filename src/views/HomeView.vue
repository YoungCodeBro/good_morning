<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Plan msg="Welcome to Your Vue.js App"/>
    <Calculator msg="Welcome to Your Vue.js App"/>
    <Food msg="Welcome to Your Vue.js App"/>
    <Food msg="Welcome to Your Vue.js App"/>
    <Food msg="Welcome to Your Vue.js App"/>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Plan from '@/components/plan.vue'
import Calculator from '@/components/calculator.vue'
import Food from '@/components/food.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    Plan,
    Calculator,
    Food
  }
}
</script>

<style lang="scss" scoped>
.b_red {
  border: solid 1px red;
}
</style>
