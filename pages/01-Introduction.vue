<template>
  <main>
    <header>Header</header>
    <aside>Left</aside>
    <article>Content</article>
    <aside>Right</aside>
    <footer>Footer</footer>
  </main>
</template>

<style scoped>
main > * {
  background-color: goldenrod;
  padding: 10px;
  font-size: 3em;
}

main {
  display: grid;
  grid-gap: 10px;

  grid-template-areas:
    "header"
    "left"
    "content"
    "right"
    "footer";
}

@media (min-width: 500px) {
  main {
    grid-template-areas:
      "header header header"
      "left content right"
      "footer footer footer";
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
