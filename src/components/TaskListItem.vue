<script>
export default {
  props: {
    completed: {
      type: Boolean,
      default: false
    },
    label: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <li>
    <div class="view">
      <input type="checkbox" class="toggle" v-model="completed" />
      <label>{{ label }}</label>
      <button class="destroy"></button>
    </div>
    <input type="text" class="edit" />
  </li>
</template>

<style></style>
