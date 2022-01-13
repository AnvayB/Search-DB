<template>
  <div class="links">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300&display=swap" rel="stylesheet">
  </div>
  <div class="app">
    <header>
      <h1>The<strong>Anime</strong>Database</h1>
    </header>
  </div> 
</template>

<script>


export default {
  name: 'app',
  query: ''
  
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto Condensed', sans-serif;
}

a {
  text-decoration: none;
}
#app {
  
}

header {
  padding-top: 50px;
  padding-bottom: 50px;

}
header h1 {
  color: #888;
  font-size: 42px;
  font-weight: 400;
  text-align: center;
  text-transform: uppercase;
}
header h1 strong {
  color: black;
}
header h1:hover {
  color: #313131;
}
</style>
