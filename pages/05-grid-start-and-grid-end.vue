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
    [sidebar-end content-start] 2fr
    [content-end];

  grid-template-rows:
    [header-start] 1fr
    [header-end content-start] 2fr
    [footer-start] 1fr
    [footer-end];
}

main > * {
  font-family: sans-serif;
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
}

header {
  grid-column: sidebar-start / content-end;
}

aside {
  grid-row: header-end / footer-end;
}

footer {
  grid-column: content-start / content-end;
}
</style>
