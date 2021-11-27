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
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  grid-template-columns: repeat(auto-fit, minmax(30px, auto));
}

main > * {
  order: 1;
}

main div {
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: sans-serif;
}

main div:nth-child(4) {
  background-color: purple;
  color: white;
  order: 1;
}
</style>
