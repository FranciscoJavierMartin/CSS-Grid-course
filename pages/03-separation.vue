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

<style scoped>
main {
  height: 100vh;
  display: grid;
  grid-gap: 10px 30px;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);
  grid-auto-rows: 1fr;
}

main div {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: purple;
  color: white;
}
</style>
