<script setup lang="ts">
import AddTodos from "./AddTodos.vue";
import TodoItem from "./TodoItem.vue";
</script>

<template>
  <main>
    <section class="content">
      <div class="container">
        <todoItem />
        <div class="todo__item">
          <div class="todo__item__ok">
            <i class="fa fa-check" aria-hidden="true"></i>
          </div>
          <div class="todo__item__text">Learn the basics of Vue</div>
          <div class="todo__item__delete">
            <i class="fa fa-trash" aria-hidden="true"></i>
          </div>
        </div>
        <div class="todo__item">
          <div class="todo__item__ok">
            <i class="fa fa-check" aria-hidden="true"></i>
          </div>
          <div class="todo__item__text">Learn the basics of Vue</div>
          <div class="todo__item__delete">
            <i class="fa fa-trash" aria-hidden="true"></i>
          </div>
        </div>
        <AddTodos />
      </div>
    </section>
  </main>
</template>
