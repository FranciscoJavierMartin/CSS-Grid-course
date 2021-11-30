<template>
  <section class="auto-fill">
    <div>Column 1</div>
    <div>Column 2</div>
    <div>Column 3</div>
    <div>Column 4</div>
  </section>
  <section class="auto-fit">
    <div>Column 1</div>
    <div>Column 2</div>
    <div>Column 3</div>
    <div>Column 4</div>
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-gap: 10px;
  font-family: sans-serif;
  margin: 20px 0;
}

section div {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 50px;
  text-align: center;
}

.auto-fill div {
  background-color: goldenrod;
}

.auto-fit div {
  background-color: purple;
  color: white;
}

.auto-fill {
  grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
}

.auto-fit {
  grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
}
</style>
