<template>
  <div class="content">
    <div class="content-header">2018</div>
    <div class="content-inner">
      <Book
        class="book"
        v-for="index in 40"
        :key="index"
        :index="index"
        :year=2018
      />
    </div>
    <br />
    <div class="content-header">2017</div>
    <div class="content-inner">
      <Book
        class="book"
        v-for="index in 55"
        :key="index"
        :index="index"
        :year=2017
      />
    </div>
    <br />
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

.content-header {
  color: white;
  background-color: purple;
  font-weight: bold;
  font-size: 150%;
  padding: 5px 0;
  margin: 10px 20px;
}

.book {
  display: inline-block;
  margin: 5px;
}
</style>
