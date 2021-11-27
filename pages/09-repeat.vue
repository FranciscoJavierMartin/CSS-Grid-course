<template>
  <main>
    <div>Column 1</div>
    <div>Column 2</div>
    <div>Column 3</div>
    <div>Column 4</div>
    <div>Column 5</div>
    <div>Column 6</div>
    <div>Column 7</div>
    <div>Column 8</div>
    <div>Column 9</div>
    <div>Column 10</div>
    <div>Column 11</div>
    <div>Column 12</div>
  </main>
</template>

<style>
main {
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  font-family: sans-serif;
  grid-template-columns:
    [start]
    repeat(
      4,
      [col-lg-start] minmax(80px, 1fr) [col-lg-end col-md-start]
        minmax(40px, 1fr) [col-md-end col-sm-start]minmax(20px, 1fr)
    )
    [end];
}

main div {
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
}

main div:first-of-type {
  background-color: purple;
  color: white;

  grid-column: col-lg-start / col-md-end;
}
</style>
