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
  </main>
</template>

<style>
main {
  display: grid;
  height: 100vh;
  grid-gap: 10px;
  font-family: sans-serif;
  grid-template-columns: 
  /* repeat(8, 1fr);*/
  /* 8 columns with a minimun value and a maximun value */
  /* repeat(8, minmax(100px, 1fr)); */
  /* 8 columns with (30px and minimum value 10% and maximun flex) */
  /* repeat(4,30px minmax(10%, 1fr)); */
  /* 8 columns with a minimun value as the content and a maximun value of 30% */
  /* repeat(8,minmax(min-content, 30%)); */
  /* 8 columns with a minimun value as the content and a maximun value as the content */
  repeat(8, minmax(min-content, max-content));
}

main div {
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
