<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  
    
      <nav>
        <nav>
          <ul class="navigation">
            <div>
              <li class="underline"><router-link to="/" ><img class="logo" src="../src/assets/ulrika_logo_new.webp" alt=""></router-link></li>
            </div>
            <div class="links">
              <li><router-link to="/" >Hem</router-link></li>
              <li ><router-link to="/about" >Om mig</router-link></li>
              <li class="border" ><router-link to="/contact" >Kontakt</router-link></li>
            </div>
            
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
.border{
  border: 2px solid #F1C6B8;
  border-radius: 10px;
  
}
.border:hover{
  background-color:#F1C6B8 ;
  
}
.logo{
  width:180px;
}
.navigation {
  list-style: none;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap:5rem;
 
}
.navigation li{
  padding:6px 10px;
}
.navigation div:first-child{
  flex:3;
}
.navigation .links{
  display: flex;
  justify-content: space-around;
  flex:2; 
} 
.navigation li {
  margin: 0 10px;
}

.navigation .links:hover{
  cursor:pointer;
}

.navigation a {
  text-decoration: none;
  color: #333;
  font-size:14px;
}
@media screen and (max-width:600px) {
  .navigation{
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap:1rem;
  }
}
</style>
