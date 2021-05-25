<template>
  <h1>Lifecycle Hooks</h1>
</template>

<script>
export default {
  setup(){
    onMounted(() => {
      console.log('Foi montado')
    }

    )
  }
}
export default {
  mounted(){
    console.log("Foi montado option API")
  }
}
</script>

<style>

</style>