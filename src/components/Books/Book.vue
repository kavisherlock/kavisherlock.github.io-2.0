<template>
  <div class="book">
    <img :src='bookSource' />
  </div>
</template>

<script>
export default {
  name: 'Book',
  props: {
    index: Number,
    year: Number
  },
  computed: {
    bookSource() {
      let imgSrc;
      try {
        imgSrc = require(`../../resources/books/${this.year}/book${this.index}.jpeg`);
      } catch(error) {
        try {
          imgSrc = require(`../../resources/books/${this.year}/book${this.index}.jpg`);
        } catch(error2) {
          try {
            imgSrc = require(`../../resources/books/${this.year}/book${this.index}.png`);
          } catch(error3) {}
        }
      }
      return imgSrc;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.book {
  text-align: center;
  background-color: purple;
  color: white;
  width: 12.5%;
  height: 100px;
}

.book img {
  width: 100%;
}
</style>
