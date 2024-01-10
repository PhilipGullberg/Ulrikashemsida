<template>
    <div class="cards-container">
      <!-- Card for 'Vad jag gör' -->
      <div class="card">
        <h2>Vad jag gör</h2>
        <!-- List of services -->
        <ul>
          
          <li>
            <v-icon name="bi-music-player" />
           <p> Anpassade träningsprogram som passar just dig. Jag är utbildad PT med vidareutbildningar inom Zuma, etc etc.</p>


          </li>
          <li>Att bygga muskler är viktigt, men att träna upp ditt hjärta och din kondition är lika viktigt. Tillsammans ger vi oss ut i skogen och tränar!</li>
          <!-- More list items -->
          <li>Mat är livet, alla ska njuta och äta gott. Men det finns bra tips på vad man kan äta för att få ut mest av träningen, där hjälper jag till!</li>
        </ul>
      </div>
  
      <!-- Card for 'Mina utbildningar' -->
      <div class="card">
        <h2>Mina utbildningar</h2>
        <!-- List of education credentials -->
        <ul>
          <li>
            <img src="" alt="Icon 2">
            Jag har gått 3 år idrottspedagog...
          </li>
          <!-- More list items -->
        </ul>
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
    gap: 20px;
    justify-content: center;
    margin-bottom: 5rem;
  }
  
  .card {
    background: #FFFFFF;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.25);
    padding: 20px;
    width: 45%; /* You can adjust the width as needed */
  }
  
  .card h2 {
    margin-bottom: 15px;
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
  