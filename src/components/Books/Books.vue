<template>
  <div class="content">
    <div class="content-inner">
      <Book
        class="book"
        v-for="index in 120"
        :key="index"
      />
    </div>
  </div>
</template>

<script>
import Book from './Book.vue';

export default {
  name: 'Books',
  components: {
    Book,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content {
  text-align: center;
  background-color: lavender;
  width: 100%;
  padding-top: 10px;
}

.book {
  display: inline-block;
  margin: 5px;
}
</style>
