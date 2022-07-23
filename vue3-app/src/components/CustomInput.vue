<script setup>
defineProps(['modelValue'])
defineEmits(['update:modelValue'])

</script>

<template>
  <input
    class="success"
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
  />
</template>

<style>
  .success {
    color: yellow;
  }
</style>