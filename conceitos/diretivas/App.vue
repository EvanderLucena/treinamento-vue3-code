<template>
  <div>
    <h1>Lista de Task</h1>
    <button @click="() => (showList = !showList)">
     Ver Lista
    </button>
    <br>
    <input type="text" v-focus>
    <ul v-if="showList">
      <li v-for="(task, index) in tasks" :key="`${task}-${index}`">
        {{ task.name }}
      </li>
    </ul>
    <p v-else>Lista de task escondida</p>
  </div>
</template>

<script>
const focus = {
    inserted: (el) => {
        el.focus()
    }
}
export default {
    directives: {
        focus
    },
  data: () => ({
    showList: false,
    tasks: [{ name: "Fazer o curso", isDone: false }],
  }),
};
</script>

<style>
</style>