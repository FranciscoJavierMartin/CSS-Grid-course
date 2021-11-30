<template>
  <main class="main">
    <header class="header">
      <h3>CSS GRID</h3>
    </header>
    <aside class="left">Side 1</aside>
    <article class="content">
      <img
        class="content__img"
        src="https://placekitten.com/g/600/300"
        alt="Article media"
      />
      <h1>Article title</h1>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Est maiores
        pariatur ipsa eius nihil? Ipsam, aspernatur. Asperiores atque nobis iste
        tenetur, perferendis eligendi possimus sit illum facere praesentium
        impedit illo?
      </p>
    </article>
    <section class="appendix1">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque nesciunt
      tempore est esse libero, soluta corporis possimus sed vel. Consequuntur
      maxime fugiat nulla, sed blanditiis neque iusto amet vitae unde.
    </section>
    <section class="appendix2">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque nesciunt
      tempore est esse libero, soluta corporis possimus sed vel. Consequuntur
      maxime fugiat nulla, sed blanditiis neque iusto amet vitae unde.
    </section>
    <aside class="right">Side 2</aside>
    <footer class="footer">
      <small>Someone</small>
    </footer>
  </main>
</template>

<style scoped>
html * {
  box-sizing: border-box;
}

html,
body {
  height: 100%;
}

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: white;
}

.main {
  height: 100vh;
}

.main > * {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px;
}

@media (min-width: 600px) {
  .main {
    display: grid;
    grid-template-columns: 1fr 2fr 2fr;
    grid-template-rows: 1fr 3fr 3fr 1fr;
  }
}

@media (min-width: 900px) {
  .main {
    grid-template-columns: 1fr 3fr 3fr 1fr;
  }
}

.header {
  background-color: aquamarine;
}

@media (min-width: 600px) {
  .header {
    grid-column: 1 / -1;
  }
}

.content {
  background-color: aliceblue;
  flex-direction: column;
}

.content__img {
  width: 100%;
  height: auto;
}

@media (min-width: 600px) {
  .content {
    grid-column: span 2;
  }
}

.left {
  background-color: beige;
}

@media (min-width: 900px) {
  .left {
    grid-row: span 2;
  }
}

.appendix1 {
  background-color: goldenrod;
}

.appendix2 {
  background-color: darkcyan;
}

.right {
  background-color: bisque;
}

@media (min-width: 600px) {
  .right {
    grid-row: 3 / 4;
  }
}

@media (min-width: 900px) {
  .right {
    grid-column: 4;
    grid-row: 2 / 4;
  }
}

.footer {
  background-color: black;
  color: white;
}

@media (min-width: 600px) {
  .footer {
    grid-column: 1 / -1;
  }
}
</style>
