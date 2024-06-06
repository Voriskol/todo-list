<script setup lang="ts">
import type { ITodo } from "@/interfaces";
import type { PropType } from "vue";
defineProps({
  todo: {
    type: Object as PropType<ITodo>,
    required: true,
  },
});
</script>

<template>
  <div class="todo__item">
    <div class="todo__item__ok">
      <i class="fa fa-check" aria-hidden="true"></i>
    </div>
    <div
      class="todo__item__text todo__item-done"
      :class="{ 'todo__item-done': todo.completed }"
    >
      {{ todo.text }}
    </div>
    <div class="todo__item__delete">
      <i class="fa fa-trash" aria-hidden="true"></i>
    </div>
  </div>
</template>
