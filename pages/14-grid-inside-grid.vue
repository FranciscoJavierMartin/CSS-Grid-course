<template>
  <section id="grid-1">
    <div>1</div>
    <div>2</div>
    <div>3</div>
    <div>4</div>
    <div>
      <section id="grid-2">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
      </section>
    </div>
    <div>6</div>
    <div>7</div>
    <div>8</div>
    <div>9</div>
    <div>10</div>
  </section>
</template>

<style scoped>
#grid-1 {
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  grid-template-columns: repeat(auto-fit, minmax(100px, auto));
}

section div {
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: sans-serif;
}

#grid-1 > div {
  background-color: goldenrod;
}

#grid-1 > div:nth-child(5) {
  background-color: transparent;
  display: block;
}

#grid-2 {
  display: grid;
  grid-gap: 15px;
  height: 100%;
  grid-template-columns: repeat(2, 1fr);
}

#grid-2 > div {
  background-color: purple;
  color: white;
}
</style>
