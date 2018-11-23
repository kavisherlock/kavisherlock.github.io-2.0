<template>
  <div class="header">
    <h1 id="title">
      <a href="/">Kavish</a>
    </h1>
    <ul id="main-menu">
      <li><a href="#" class="selected">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#books">Books</a></li>
      <li><a href="#work">Work</a></li>
      <li><a href="#blog">Blog</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-family: 'Homemade Apple';
  font-size: 2.5em;
  margin: 0;
  padding: 20px;
}

h1 a {
  text-decoration: none;
  color: #E6E6FA;
  text-shadow:  4px 4px 3px rgb(55, 30, 78);
  transition: color 0.5s ease-in-out;
  -moz-transition: color 0.5s ease-in-out;
  -webkit-transition: color 0.5s ease-in-out;
}

h1 a:hover {
  text-decoration: none;
  text-shadow:  4px 4px 3px #555;
}

ul, ol {
  list-style: none;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

#main-menu {
  float: right;
  overflow: hidden;
  margin: -50px 50px 50px 0;
}

#main-menu li {
  display: inline;
  font-size: 1.25em;
}

#main-menu li a {
  font-family: 'Homemade Apple', cursive, sans-serif;
  font-weight: bold;
  text-decoration: none;
  display: inline-block;
  margin: 0 10px;
  padding: 5px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  border-radius: 10px;
  color: rgb(61, 61, 155);
  transition: background-color 0.5s ease-in-out;
  -moz-transition: background-color 0.5s ease-in-out;
  -webkit-transition: background-color 0.5s ease-in-out;
}

#main-menu li a.selected {
  color: #FFF;
  background-color: #3D7DB2;
}

#main-menu li a:hover {
  color: #FFF;
  background-color: #3D7DB2;
}

</style>
