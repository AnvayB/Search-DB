<template>
  <div class="links">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300&display=swap" rel="stylesheet">
  </div>
  <div class="app">
    <header>
      <h1>The<strong>Anime</strong>Database</h1>
      <form class="search-box">
        <input 
          type="search" 
          class="search-field" 
          placeholder="Search for an anime..."
          required>
      </form>
    </header>

    <main>
      <div class="cards">
        <Card />
      </div>
    </main>

  </div> 
</template>

<script>
import Card from './components/Card';
export default {
    setup() {
        return {
            Card
        }
    }
}
</script>

<style>
body:not(header h1) {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;
}


/* a {
  text-decoration: none;
} */

header {
  padding-top: 50px;
  padding-bottom: 50px;
  font-family: 'Roboto Condensed', sans-serif;

}
header h1 {
  color: #888;
  font-size: 42px;
  font-weight: 400;
  text-align: center;
  text-transform: uppercase;
  margin-bottom: 30px;
}

header h1 strong {
  color: black;
}
header h1:hover {
  color: black;
}

.search-box {
  display: flex;
  justify-content: center;
  padding-left: 30px;
  padding-right: 30px;
}
.search-box .search-field {
  appearance: none;
  background: none;
  border: none;
  outline: none;

  background-color: #f3f3f3;
  box-shadow: 4px 8px rgba(0, 0, 0, 0.15);

  display: block;
  width: 100%;
  max-width: 600px;
  padding: 15px;
  border-radius: 8px;

  font-size: 20px;
  transition: .4s;

}
.search-box .search-field::placeholder {
  color: #aaa;
}
.search-box .search-field:focus, .search-box .search-field:valid {
  color: white;
  background-color: black;
  box-shadow: 0x 0px rgba(0, 0, 0, 0.15) ;
}
</style>
