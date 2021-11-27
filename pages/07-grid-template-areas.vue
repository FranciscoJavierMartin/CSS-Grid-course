<template>
  <main>
    <header>Header</header>
    <aside>Left</aside>
    <article>Content</article>
    <aside>Right</aside>
    <footer>Footer</footer>
  </main>
</template>

<style>
main {
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  font-family: sans-serif;
  grid-template-areas:
    "header"
    "content"
    "left"
    "right"
    "footer";
}

main > * {
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (min-width: 500px) {
  main {
    grid-template-areas:
      "header header right"
      "left content right"
      "left footer right";
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-rows: 2fr 5fr 1fr;
  }
}

header {
  grid-area: header;
}

aside:first-of-type {
  grid-area: left;
}

article {
  grid-area: content;
}

aside:last-of-type {
  grid-area: right;
}

footer {
  grid-area: footer;
}
</style>
