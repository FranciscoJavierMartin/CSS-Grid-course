<template>
  <main>
    <section>Element 001</section>
    <section>Element 002</section>
    <section>Element 003</section>
    <section>Element 004</section>
    <section>Element 005</section>
    <section>Element 006</section>
    <section>Element 007</section>
    <section>Element 008</section>
    <section>Element 009</section>
    <section>Element 010</section>
    <section>Element 011</section>
    <section>Element 012</section>
    <section>Element 013</section>
    <section>Element 014</section>
    <section>Element 015</section>
    <section>Element 001</section>
    <section>Element 002</section>
    <section>Element 003</section>
    <section>Element 004</section>
    <section>Element 005</section>
    <section>Element 006</section>
    <section>Element 007</section>
    <section>Element 008</section>
    <section>Element 009</section>
    <section>Element 010</section>
    <section>Element 011</section>
    <section>Element 012</section>
    <section>Element 013</section>
    <section>Element 014</section>
    <section>Element 015</section>
    <section>Element 001</section>
    <section>Element 002</section>
    <section>Element 003</section>
    <section>Element 004</section>
    <section>Element 005</section>
    <section>Element 006</section>
    <section>Element 007</section>
    <section>Element 008</section>
    <section>Element 009</section>
    <section>Element 010</section>
    <section>Element 011</section>
    <section>Element 012</section>
    <section>Element 013</section>
    <section>Element 014</section>
    <section>Element 015</section>
    <section>Element 001</section>
    <section>Element 002</section>
    <section>Element 003</section>
    <section>Element 004</section>
    <section>Element 005</section>
    <section>Element 006</section>
    <section>Element 007</section>
    <section>Element 008</section>
    <section>Element 009</section>
    <section>Element 010</section>
    <section>Element 011</section>
    <section>Element 012</section>
    <section>Element 013</section>
    <section>Element 014</section>
    <section>Element 015</section>
    <section>Element 001</section>
    <section>Element 002</section>
    <section>Element 003</section>
    <section>Element 004</section>
    <section>Element 005</section>
    <section>Element 006</section>
    <section>Element 007</section>
    <section>Element 008</section>
    <section>Element 009</section>
    <section>Element 010</section>
    <section>Element 011</section>
    <section>Element 012</section>
    <section>Element 013</section>
    <section>Element 014</section>
    <section>Element 015</section>
  </main>
</template>

<style scoped>
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
  background-color: white;
}

main {
  width: 100vw;
  height: 100vh;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  grid-template-rows: repeat(auto-fit, minmax(150px, 1fr));
  grid-auto-rows: minmax(150px, 1fr);
  grid-auto-columns: minmax(150px, 1fr);
  grid-auto-flow: column dense;
}

section {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: goldenrod;
  border: 1px solid black;
}
</style>
