<template>
  <input :value="value" @input="onChange"  />
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: ''
    }
  },
  methods: {
    onChange(e) {
      this.$emit('input', e.target.value)
    }
  },
}
</script>

<style>
</style>