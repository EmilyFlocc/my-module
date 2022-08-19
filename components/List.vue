<template>
  <div class="container">
    <p>List here: {{ posts }}</p>
    <h2>For loop below:</h2>
    <div
      v-for="item in posts"
      :key="item.id"
    >
      <p>{{ item.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    posts: {
      type: Array,
      default: null
    }
  }
}
</script>
