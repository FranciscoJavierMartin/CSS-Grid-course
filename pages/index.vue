<template>
  <main>
    <h1>CSS Grid course</h1>
    <div class="grid">
      <div class="lesson" v-for="(lesson, index) in links" :key="index">
        <nuxt-link :to="lesson.link">{{ lesson.text }}</nuxt-link>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  computed: {
    links() {
      return [
        {
          text: "Introduction",
          link: "01-introduction",
        },
        {
          text: "Terminology",
          link: "02-terminology",
        },
        {
          text: "Separation",
          link: "03-separation",
        },
        {
          text: "Grid lines by name",
          link: "04-grid-lines-by-name",
        },
        {
          text: "Grid-start and grid-end",
          link: "05-grid-start-and-grid-end",
        },
        {
          text: "Grid-start and grid-end",
          link: "06-grid-start-and-grid-end",
        },
        {
          text: "Grid template areas",
          link: "07-grid-template-areas",
        },
        {
          text: "Limits with minmax",
          link: "08-limits-with-minmax",
        },
        {
          text: "Repeat",
          link: "09-repeat",
        },
        {
          text: "Dynamic grid with auto-fill and auto-fit",
          link: "10-dynamic-grid-with-auto-fill-and-auto-fit",
        },
        {
          text: "Grid auto placement and packing modes",
          link: "11-grid-auto-placement-and-packing-modes",
        },
        {
          text: "Implicit and explicit grid",
          link: "12-implicit-and-explicit-grid",
        },
        {
          text: "Reorder grid items",
          link: "13-reorder-grid-items",
        },
        {
          text: "Grid inside grid",
          link: "14-grid-inside-grid",
        },
        {
          text: "Grid template",
          link: "15-grid-template",
        },
        {
          text: "Grid",
          link: "16-grid",
        },
        {
          text: "Grid align items with justify-items",
          link: "17-grid-align-items-with-justify-items",
        },
        {
          text: "Grid align items with align-items",
          link: "18-grid-align-items-with-align-items",
        },
        {
          text: "Grid align items with justify-self",
          link: "19-grid-align-items-with-justify-self",
        },
        {
          text: "Grid align items with align-self",
          link: "20-grid-align-items-with-align-self",
        },
      ];
    },
  },
};
</script>
<style scoped>
main {
  font-family: sans-serif;
}

h1 {
  text-align: center;
}

.grid {
  display: grid;
  grid-template-columns: 1fr;
  justify-items: stretch;
  align-items: stretch;
}

.lesson {
  background-color: goldenrod;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 100px 50px;
  margin: 10px;
  border-radius: 20px;
  font-size: 20px;
}

@media (min-width: 576px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 768px) {
  .grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

.lesson:hover {
  background-color: purple;
}

a {
  text-decoration: none;
  color: white;
}
</style>
