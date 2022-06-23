<script></script>
<template>
  <header class="menu-superior">
      <div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" >
   Menu
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
    <li><RouterLink to="/">Home</RouterLink></li>
    <li><RouterLink to="/about">Sobre</RouterLink></li>
  </ul>
</div>


<div class="pesquisar">
  <nav class="navbar">
  <div class="container-fluid">
    <form class="d-flex" role="search">
      <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-primary" type="submit">Search</button>
    </form>
  </div>
</nav>
</div>


<div id="bola"></div>
  </header>
  <main><router-view /></main>
  <footer>rodapé</footer>
</template>

<style>
@import "@/assets/style.css";
@import "@/assets/style.css";
#app {
  max-width: 1920px;
  margin: auto;
  height: 100vh;
  font-weight: normal;
}



header .menu-superior{
  justify-content: space-between;
  display: flex;
  align-items: center;
}

.pesquisar{
  padding-left: 20px;
  background-color: #d9d9d9;
}
.pesquisar input{
  padding: 0 250px;
}

header,
footer {
  height: 15%;
  display: flex;
  align-items: center;
  border: 1px black solid;
  background-color: #d9d9d9;
  
}
main {
  height: 70%;
  background-color: #d9d9d9;
}
.dropdown {
  display: flex;
  padding-left: 20px;
}
#bola {
    border-radius: 50%;
    display: inline-block;
    height: 70px;
    width: 70px;
    border: 1px solid #000000;
    background-color: gray;
    margin-left: 500px;
}


</style>
