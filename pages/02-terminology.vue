<template>
  <main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
    <div>4</div>
    <div>5</div>
    <div>6</div>
    <div>7</div>
    <div>8</div>
    <div>9</div>
    <div>10</div>
  </main>
</template>

<style>
main {
  height: 100vh;
  display: grid;
  grid-gap: 20px;
  grid-template-columns: repeat(4, 100px);
  grid-template-rows: repeat(3, 100px);
}

main div {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: goldenrod;
}

@media (max-width: 600px) {
  div:nth-child(6) {
    background-color: purple;
    grid-column: 2/3;
    grid-row: 2/4;
  }

  div:nth-child(10) {
    background-color: purple;
    /* grid-column-start: 3;
  grid-column-end: 5; */
    /* Shortcut */
    grid-column: 3 / 5;
  }
}
</style>
