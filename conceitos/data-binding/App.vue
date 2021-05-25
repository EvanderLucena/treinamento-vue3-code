<template>
<div>
  <h1 :style="{textDecoration: decoration}">Vue Js: {{name}}</h1>
  <input type="text" v-model="name">
  <br>
  <a :href="link">github</a>
</div>
</template>

<script>
export default {
    data: () => ({
        name: 'DataBinding',
        link: 'https://github.com/EvanderLucena',
        decoration:'underline'
    })
}
</script>

<style>

</style>