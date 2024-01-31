
<template>
  <div class="app-container">
   
    <main>
      
      <section class="intro">
        
        <p>Träning för Livets Njutning</p>
        
      
        <div class="description">
          <p>Dyk in i världen av hälsa och personlig träning med Ulrika Andersson.
Här handlar det om att öka livet genom fysisk aktivitet och välmående.
Uppskräddarsydda träningsprogram och motivation för att skapa en hälsosammare och gladare livsstil.</p>
        </div>
        <router-link to="/contact" class="no-underline">
          <button class="cssbuttons-io-button">
            <span>Kontakta mig</span>
            <div class="icon">
              <svg
                height="24"
                width="24"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path d="M0 0h24v24H0z" fill="none"></path>
                <path
                  d="M16.172 11l-5.364-5.364 1.414-1.414L20 12l-7.778 7.778-1.414-1.414L16.172 13H4v-2z"
                  fill="currentColor"
                ></path>
              </svg>
            </div>
          </button>
          </router-link>

      </section>
      <section class="profile-image">
        <img class="blob" src="../assets/blob.svg" alt="">
           
        <img src="../assets/Ulrika.webp" class="blob-mask" alt="">
        <!-- Image will be placed as a background in CSS -->
      </section>
      
    </main>
  </div>
  <div class="arrow">
  <svg width="377" height="122" viewBox="0 0 377 122" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M368 122L376.379 100.48L353.553 103.983L368 122ZM362.921 88.9052L360.944 89.2086L362.921 88.9052ZM287.725 75.8051L288.862 74.1598L287.725 75.8051ZM1.55486 43.1193L122.891 8.08169L121.781 4.2387L0.445139 39.2763L1.55486 43.1193ZM205.796 21.6146L286.588 77.4504L288.862 74.1598L208.07 18.324L205.796 21.6146ZM360.944 89.2086L363.293 104.512L367.246 103.905L364.898 88.6018L360.944 89.2086ZM321.229 75.1429C335.339 62.3164 358.051 70.3601 360.944 89.2086L364.898 88.6018C361.521 66.6 335.01 57.2107 318.538 72.183L321.229 75.1429ZM286.588 77.4504C297.266 84.8304 311.623 83.8741 321.229 75.1429L318.538 72.183C310.309 79.6628 298.01 80.4821 288.862 74.1598L286.588 77.4504ZM122.891 8.08169C151.156 -0.0804208 181.593 4.88792 205.796 21.6146L208.07 18.324C182.879 0.914578 151.2 -4.25655 121.781 4.2387L122.891 8.08169Z" fill="#F1C6B8"/>
    </svg>
  </div>

  <AboutMe />
  <div class="banner">
    <h2>Vill du veta mer?</h2>
    <router-link to="/contact"> <button class="banner_button">Kontakta mig nu</button> </router-link>
  </div>
  <Testimony />
  <MyWork />
  
</template>

<script>
import AboutMe from '../components/AboutMe.vue';
import Testimony from '../components/Testimony.vue';
import MyWork from '../components/MyWork.vue';


export default {
  name: 'App',
  components: {
    // Register the component
    AboutMe,Testimony, MyWork
  }
  // component logic
}
</script>

<style scoped>
.no-underline{
  text-decoration: none;
}
.app-container {
  font-family: 'Open Sans', sans-serif;
 
}
.banner_button{
  background-color: white;
  color:black;
  cursor: pointer;
  padding:1rem;
  border-radius: 8px;
  border:none;
  font-size: 16px;
  box-shadow: 1px 2px 4px 4px #00000020;
}
.banner_button:hover{
 transform: translate(1px,1px);
}
.banner{
  height: 100px;
  border-radius: 8px;
  display:flex;
  justify-content: center;
  align-items: center;
  background-color: #F1C6B8;
  width:100%;
  gap:10rem;
  margin-bottom:4rem;
}
 
main{
  display:flex;
  justify-content: space-around;
  margin-top:5rem;
  
}
.intro {
  text-align: center;
  padding: 2em;
  padding-top:0rem;
  display:flex;
  flex-direction: column;
  

}
.intro h1{
  font-size:48px;
}
.intro p{
  font-size: 36px;
  font-weight: bold;
  
}
.arrow{
  display: flex;
  justify-content: center;
  margin-right:10rem;
  margin-top:2rem;
}
.description{
  padding:0rem 4rem 0rem 4rem;
}
.description p {
  color: #555;
  line-height: 1.6;
  font-size: 18px;
  
  font-weight: normal;
 
}

.contact-btn {
  background-color: #F1C6B8;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  font-size: 1em;
  color: rgb(0, 0, 0);
  margin-top: 20px;
  border-radius: 5px;
}


.profile-image{
  position: relative;
  z-index:1;
}
.profile-image img {
  border-radius: 8px;
  width:300px;

}
.rainbow{
  position: relative;
}
svg.rainbow{
  position: absolute;
  left:50px;
  bottom:60px;
}
.cssbuttons-io-button {
  background: #F1C6B8;
  color: black;
  
  font-family: inherit;
  padding: 0.35em;
  padding-left: 1.2em;
  font-size: 16px;
  font-weight: 500;
  border-radius: 0.9em;
  border: 1px solid rgba(44, 44, 44, 0.115);
  letter-spacing: 0.05em;
  display: flex;
  align-items: center;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  overflow: hidden;
  position: relative;
  height: 2.8em;
  padding-right: 3.3em;
  cursor: pointer;
}

.cssbuttons-io-button .icon {
  background: white;
  margin-left: 1em;
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2.2em;
  width: 2.2em;
  border-radius: 0.7em;
  box-shadow: 0.1em 0.1em 0.6em 0.2em #f6dad0;
  right: 0.3em;
  transition: all 0.3s;
}

.cssbuttons-io-button:hover .icon {
  width: calc(100% - 0.6em);
}

.cssbuttons-io-button .icon svg {
  width: 1.1em;
  transition: transform 0.3s;
  color: black;
}

.cssbuttons-io-button:hover .icon svg {
  transform: translateX(0.1em);
}

.cssbuttons-io-button:active .icon {
  transform: scale(0.95);
}

 .rainbow-arch {
            fill: none; /* No fill to create just an outline */
            stroke: #F1C6B8; /* Border color */
            stroke-width: 5; /* Border width */
        }


img.blob{
 position: absolute;
  z-index: -1;
  width:500px;
  top:-5rem;
  left:1rem;
  
}
@media (max-width: 800px) {
   .profile-image {
    width: 50%;
    display: none;
  }
  main{
    flex-direction: column;
    margin-top: 1rem;
    justify-content: center;
    align-items: center;
  
  }
  .banner{
    gap:1rem;
    flex-direction: column;
    height:150px;
  }

  .intro {
    display: flex;
    align-items: center;
    justify-content: space-around;
  }
  .description{
    padding:0rem;
    padding-top:1rem;
    padding-bottom: 1rem;
  }
  
}

@media (min-width: 768px) {
  .intro {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    flex:2;
    margin-top: 1rem;
  }
  .profile-image{
    flex:1;
  }
  main{
    width:100%;
    justify-content: space-around;
  }
 
  
  
}

</style>
