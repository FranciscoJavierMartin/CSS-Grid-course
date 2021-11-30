<template>
  <main>
    <header>Header</header>
    <aside>Left</aside>
    <article>Content</article>
    <aside>Right 1</aside>
    <aside>Right 2</aside>
    <footer>Footer</footer>
  </main>
</template>

<style scoped>
main {
  height: 100vh;
  display: grid;
  grid-gap: 10px;
  font-family: sans-serif;
  /* grid-template-areas:
    "header header header"
    "left content right1"
    "left content right2"
    "left footer footer";
  grid-template-rows: [start] 1fr [content-start] 2fr 1fr 1fr [end];
  grid-template-columns: [start] 1fr [content-start] 2fr 1fr [end]; */
  grid-template: 
  /* Rows */
    [start] "header header header" 1fr
    [content-start] "left content right1" 2fr
    "left content right2" 1fr
    "left footer footer" 1fr [end]
    /
    /* Columns */
    [start] 1fr [content-start] 2fr 1fr [end];
}

main > * {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: goldenrod;
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

aside:nth-of-type(2) {
  grid-area: right1;
}

aside:last-of-type {
  grid-area: right2;
}

footer {
  grid-area: footer;
}
</style>
