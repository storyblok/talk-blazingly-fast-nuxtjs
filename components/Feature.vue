<template>
  <div
    v-editable="blok"
    class="text-center">
    <h2 class="text-xl font-medium">{{ blok.name }}</h2>
  </div>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>
