
<template>
  <div class="app-container">
   
    <main>
      <section class="profile-image">
        <img src="../assets/muddyullis.png" alt="">
      </section>
      <section class="intro">
  
        <p>Ulrika Andersson, Träning för Livets Njutning</p>
        <div class="description">
          <p>Dyk in i världen av hälsa och personlig träning med Ulrika Andersson.</p>
          <p>Här handlar det om att öka livet genom fysisk aktivitet och välmående.</p>
          <p>Uppskräddarsydda träningsprogram och motivation för att skapa en hälsosammare och gladare livsstil.</p>
        </div>
        <button class="contact-btn">Kontakta mig</button>
      </section>
      <section class="profile-image">
        <img src="../assets/Ulrika.png" alt="">
        <!-- Image will be placed as a background in CSS -->
      </section>
      
    </main>
  </div>
  <div class="arrow">
  <svg width="377" height="122" viewBox="0 0 377 122" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M368 122L376.379 100.48L353.553 103.983L368 122ZM362.921 88.9052L360.944 89.2086L362.921 88.9052ZM287.725 75.8051L288.862 74.1598L287.725 75.8051ZM1.55486 43.1193L122.891 8.08169L121.781 4.2387L0.445139 39.2763L1.55486 43.1193ZM205.796 21.6146L286.588 77.4504L288.862 74.1598L208.07 18.324L205.796 21.6146ZM360.944 89.2086L363.293 104.512L367.246 103.905L364.898 88.6018L360.944 89.2086ZM321.229 75.1429C335.339 62.3164 358.051 70.3601 360.944 89.2086L364.898 88.6018C361.521 66.6 335.01 57.2107 318.538 72.183L321.229 75.1429ZM286.588 77.4504C297.266 84.8304 311.623 83.8741 321.229 75.1429L318.538 72.183C310.309 79.6628 298.01 80.4821 288.862 74.1598L286.588 77.4504ZM122.891 8.08169C151.156 -0.0804208 181.593 4.88792 205.796 21.6146L208.07 18.324C182.879 0.914578 151.2 -4.25655 121.781 4.2387L122.891 8.08169Z" fill="#EEB45E"/>
    </svg>
  </div>

  <AboutMe />
  <MyWork />
  <ImageGrid />
</template>

<script>
import AboutMe from '../components/AboutMe.vue';
import ImageGrid from '../components/ImageGrid.vue';
import MyWork from '../components/MyWork.vue';

export default {
  name: 'App',
  components: {
    // Register the component
    AboutMe,ImageGrid, MyWork
  }
  // component logic
}
</script>

<style scoped>
.app-container {
  font-family: 'Open Sans', sans-serif;
 
}
main{
  display:flex;
  justify-content: space-between;
  margin-top:5rem;
}
.intro {
  text-align: center;
  padding: 2em;
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
  margin-top:2rem;
}
.description{
  margin-top: 0.5rem;
}
.description p {
  color: #555;
  line-height: 1.6;
  font-size: 15px;
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

.profile-image img {
  border-radius: 8px;
  width:300px;
  margin-left:3rem;
}

@media (min-width: 768px) {
  .intro {
    display: flex;
    align-items: center;
    justify-content: space-around;
  }
  .profile-image {
    width: 50%;
  }
}

</style>
