<template>
  <div>
    <header>
      <slot name="header"></slot>
    </header>
    <slot></slot>
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
