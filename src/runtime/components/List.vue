<template>
  <div class="w-r24/24 mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-medium">
      <div
        v-for="item in posts"
        :key="item.id"
      >
        <p>{{ item.title }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    posts: {
      type: Array,
      default: null
    },
    dates: {
      type: Object,
      default: null
    },
    canBook: {
      type: Boolean,
      default: false
    }
  }
}
</script>
