<template>
    <div><input :value="props.modelValue" @input="updateValue($event.target.value)" type="text"></div>
</template>

<script setup>
const props = defineProps({
  modelValue: String
})

const emit = defineEmits(['update:modelValue'])

function updateValue(value) {
  emit('update:modelValue', value)
}
</script>