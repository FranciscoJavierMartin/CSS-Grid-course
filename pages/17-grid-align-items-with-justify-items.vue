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
    <div>11</div>
    <div>12</div>
  </main>
</template>

<style>
main {
  display: grid;
  grid-gap: 10px;
  font-family: sans-serif;
  grid-template: repeat(4, 50px) / repeat(3, 1fr);
  justify-items: stretch;
}

main div {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: goldenrod;
}
</style>
