<template>
  <main>
    <header>Header</header>
    <aside>Sidebar</aside>
    <article>Content</article>
    <footer>Footer</footer>
  </main>
</template>

<style scoped>
main {
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  /* grid-template-columns: 1fr 2fr; */

  grid-template-columns:
    [sidebar-start] 1fr
    [content-start] 2fr;

  grid-template-rows:
    [header-start] 1fr
    [content-start] 2fr
    [footer-start] 1fr;
}

main > * {
  font-family: sans-serif;
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
}

header {
  grid-column: sidebar-start / span 2;
}

aside {
  grid-row: content-start / span 2;
}

footer {
  grid-column: content-start;
}
</style>
