<script setup lang="ts"></script>

<template>
  <header class="header">
    <div class="container">
      <h1 class="header__title">TODOS</h1>
      <nav class="navPanel">
        <section class="nav__elements">
          <button class="nav__button">All</button>
          <button class="nav__button">Active</button>
          <button class="nav__button">Done</button>
        </section>
      </nav>
    </div>
  </header>
  <main>
    <section class="content">
      <div class="container">
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
        <div class="todo__item">
          <div class="todo__item__ok">
            <i class="fa fa-check" aria-hidden="true"></i>
          </div>
          <div class="todo__item__text">Learn the basics of Vue</div>
          <div class="todo__item__delete">
            <i class="fa fa-trash" aria-hidden="true"></i>
          </div>
        </div>
        <div class="add__todos">
          <div class="add__todos__btn">
            <i class="fa fa-plus-square-o" aria-hidden="true"></i>
          </div>
          <div class="add__form">
            <div class="add__form__close">
              <i class="fa fa-times" aria-hidden="true"></i>
            </div>
            <div class="add__form__name"></div>
            <button class="add__form__btn">Add task</button>
          </div>
        </div>
      </div>
    </section>
  </main>
  <footer>
    <div class="container">
      <p>4 more to do, 0 done</p>
    </div>
  </footer>
</template>

<style scoped>
.container {
  width: 300px;
  margin: 0 auto;
}
.header {
  text-align: center;
}
.header__title {
  font-size: 3rem;
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
}
.todo__item__ok {
}
.fa {
}
.fa-check {
}
.todo__item__text {
}
.todo__item__delete {
}
.fa-trash {
}
.add__todos {
}
.add__todos__btn {
}
.fa-plus-square-o {
}
.add__form {
  display: none;
}
.add__form__close {
}
.fa-times {
}
.add__form__name {
}
.add__form__btn {
}

footer {
  text-align: center;
  opacity: 0.2;
}
</style>
