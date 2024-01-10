<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  
    
      <nav>
        <nav>
          <ul class="navigation">
            <li><a href="#training">Träning</a></li>
            <li><a href="#about-me">Om mig</a></li>
            <li><a href="#contact">Kontakt</a></li>
          </ul>
        </nav>
        
      </nav>
   

  <RouterView />
</template>

<style scoped>

header {
  background-color: #fff;
  padding: 1em;
}

.navigation {
  list-style: none;
  display: flex;
  justify-content: center;
  gap:5rem;
}

.navigation li {
  margin: 0 10px;
}

.navigation a {
  text-decoration: none;
  color: #333;
}

</style>
