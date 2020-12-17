<template>
  <div class="container">
    <div>
      <h2>Todo List</h2>
    </div>
    <todo-list></todo-list>
  </div>
</template>



<script>
// @ is an alias to /src
import TodoList from "@/components/TodoList.vue";

export default {
  name: "App",
  components: {
    TodoList,
  }
};
</script>


<style lang="scss">

h2 { color: #111; font-family: 'Open Sans', sans-serif; font-size: 30px; font-weight: 300; line-height: 32px; margin: 0 0 72px; text-align: center; }

* {
  box-sizing: border-box;
}

.container{
  max-width: 600px;
  margin: 0 auto;
}


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;*/
  color: #2c3e50;
  font-size: 24px;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

</style>
