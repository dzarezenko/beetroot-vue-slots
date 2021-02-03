<template>
  <div>
    <header>
      <h1>{{ title }}</h1>
    </header>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    text: String,
  }
}
</script>

<style scoped>
div {
  display: block;
  width: 300px;
  border: 1px solid black;
  margin-bottom: 15px;
  padding: 10px;
}
</style>
