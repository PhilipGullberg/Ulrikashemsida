<template>
    <div class="cards-container">
      <!-- Card for 'Vad jag gör' -->
      <div class="card">
        <h2>Vad jag gör</h2>
        

        <div class="box"><div class="rectangle"></div></div>
        <!-- List of services -->
        <ul>
          
          <li>
            <font-awesome-icon icon="fa-solid fa-person-running" /><p> Anpassade träningsprogram som passar just dig. Jag är utbildad PT med vidareutbildningar inom Zuma, etc etc.</p>


          </li>
          <li><font-awesome-icon icon='fa-solid fa-dumbbell' />Att bygga muskler är viktigt, men att träna upp ditt hjärta och din kondition är lika viktigt. Tillsammans ger vi oss ut i skogen och tränar!</li>
          <!-- More list items -->
          <li><font-awesome-icon icon="fa-solid fa-seedling" />Mat är livet, alla ska njuta och äta gott. Men det finns bra tips på vad man kan äta för att få ut mest av träningen, där hjälper jag till!</li>
        </ul>
      </div>
  
      <!-- Card for 'Mina utbildningar' -->
      <div class="card">
        <h2>Mina utbildningar</h2>
        <div class="box"><div class="rectangle"></div></div>
        <!-- List of education credentials -->
        <div class="image-grid">
          <img src="C:\Users\philip.gullberg\Desktop\Ulrikas Hemsida\vue-project\src\assets\411144219_6877318882386055_5022940134116447408_n (1).jpg" alt="">
          <img src="C:\Users\philip.gullberg\Desktop\Ulrikas Hemsida\vue-project\src\assets\411224089_378068304768285_6201941777321531040_n (1).jpg" alt="">
          <img src="C:\Users\philip.gullberg\Desktop\Ulrikas Hemsida\vue-project\src\assets\411249415_756274495831431_6874976518154502510_n (1).jpg" alt="">
          <img src="C:\Users\philip.gullberg\Desktop\Ulrikas Hemsida\vue-project\src\assets\413790595_746263876976475_2447653846280127914_n (1).jpg" alt="">
        </div>
      </div>
    </div>
  </template>
  
<script>

export default {
  name: 'MyWork',
  // component logic here
}
  </script>
  
  <style scoped>
  .cards-container {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: space-around;
    margin-bottom: 5rem;
  }
  .card h2 {
    font-weight: bold;
  }
  .image-grid{
    display:flex;
    flex-wrap: wrap;
    gap:10px;
    justify-content: space-around;

  }
  img{
    width:30%;
  }
  li{
    display:flex;
    gap:2rem;
    
    padding-bottom:1rem;
  
  }
  .box {
    width: 150px;
    height: 7px;
    background-color: #f1c6b8;
    margin-bottom: 20px;
  }
  .card {
    background: #FFFFFF;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.25);
    padding: 25px;
    width: 46%; /* You can adjust the width as needed */
  }
  
  
  
  .card ul {
    list-style: none;
    padding: 0;
  }
  
  .card li {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .card li img {
    margin-right: 10px;
    width: 24px; /* Adjust the size as needed */
  }
  </style>
  