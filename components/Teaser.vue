<template>
  <h2
    v-editable="blok"
    class="py-10 font-serif text-3xl text-center">
    {{ blok.headline }}
  </h2>
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
