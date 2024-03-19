<script >
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/FormView">Form</RouterLink>
      </nav>
  </header>

  <RouterView />
</template>

<style>
html, body{
  margin: 0;
  padding: 0;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

header{
  background-color: #444;
  
  
}

header nav{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 7vh;
}

nav a{
  color: #40BC83;
  text-decoration: none;
  font-size: 4vh;
  padding: 2vh;
}

nav a:hover{
  color: #51cD94;
}
</style>
