<script setup lang="ts">
import { computed } from "vue";
const props = defineProps<{
  label?: string;
  modelValue?: string;
}>();
const emit = defineEmits(["update:modelValue"]);
const _modelValue = computed({
  get() {
    return props.modelValue || "";
  },
  set(value: string) {
    emit("update:modelValue", value);
  },
});
</script>
<template>
  <label class="mb-3 block">
    <span
      v-if="label"
      class="block text-2xl text-gray-800 after:text-red-600 after:content-['*']"
      >{{ label }}</span
    >
    <input
      v-model="_modelValue"
      placeholder="alanmaldonado"
      type="text"
      required="true"
      class="block w-full rounded-lg border border-gray-400 p-3 placeholder:text-sm placeholder:italic focus:outline-lime-600 disabled:opacity-50"
    />
  </label>
</template>
