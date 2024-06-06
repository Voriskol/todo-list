<script setup lang="ts">
import TheHeader from "./components/TheHeader.vue";
import TodoList from "./components/TodoList.vue";
import TheFooter from "./components/TheFooter.vue";
</script>

<template>
  <TheHeader />
  <TodoList />
  <TheFooter />
</template>

<style>
.container {
  width: 350px;
  margin: 0 auto;
}
.header {
  text-align: center;
}
.header__title {
  font-size: 2rem;
  color: red;
}
.navPanel {
  display: flex;
  flex-direction: column;
  margin-top: 30px;
}
.nav__elements {
  border: 1px solid #d0cfcf;
  border-radius: 1rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}

.nav__button {
  font-size: 1.2rem;
  border-radius: 1rem;
  background-color: #fff;
  border: 2px solid transparent;
  padding: 0.4rem 1rem;
}

.nav__button:hover {
  border-radius: 1rem;
  border: 2px solid red;
}

.content {
  margin-top: 30px;
}
.todo__item,
.add__todos {
  margin: 20px 0;
  border: 1px solid #d0cfcf;
  border-radius: 1rem;
  display: flex;
  justify-content: space-around;
  padding: 0.4rem 1rem;
  font-size: 1.2rem;
  cursor: pointer;
}
.todo__item__ok {
  color: greenyellow;
}

.todo__item-done {
  text-decoration: line-through;
}
.todo__item__delete {
  color: rgb(213, 216, 216);
}

.add__todos {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-size: 1.4rem;
  color: rgb(141, 142, 142);
}
.add__todos__btn {
}

.add__form {
  display: flex;
  flex-direction: column;
  gap: 1.2rem;
  width: 100%;
}
.add__form__close {
  display: flex;
  justify-content: end;
}

.add__form__name {
  border: 1px solid red;
  border-radius: 1rem;
  height: 1.8rem;
  text-align: center;
}

.add__form__btn {
  font-size: 1.2rem;
  border-radius: 1rem;
  background-color: #fff;
  border: 2px solid red;
  padding: 0.2rem 0;
}
.add__form__btn:hover {
  transition: 0.3s;
  background-color: red;
  color: #fff;
}

footer {
  text-align: center;
  opacity: 0.2;
}
</style>
