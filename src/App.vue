<template>
  <div id="app">
    <div class="hello-world">
      <img alt="Vue logo" src="./assets/logo.png" />
      <div class="hello-world__message">
        {{ message }}
      </div>
    </div>
    <TodoList></TodoList>
    <Counter v-bind:initialValue="1000"></Counter>
  </div>
</template>

<script>
import TodoList from "@/components/TodoList.vue"
import Counter from "@/components/Counter.vue"
export default {
  name: "App",
  components: {
    TodoList,
    Counter,
  },
  data: function () {
    return {
      message: "WebExpert Course Vue Template",
    }
  },
  methods: {},
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
