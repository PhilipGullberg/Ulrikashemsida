<template>
    <div class="cards-container">
      <!-- Card for 'Vad jag gör' -->
      <div>
            <h1>Vad jag gör</h1>

          <div class="box"><div class="rectangle"></div></div>
            <div class="info-cols">
              <div class="col">
                <div> 
                  <font-awesome-icon icon="fa-solid fa-person-running" size="xl" pull="left" />
                  <h2>Träningsprogram</h2>
                </div>
               
                <p>Oavsett din erfarenhetsnivå skräddarsyr jag personliga träningsprogram baserade på dina unika mål och behov. Med fokus på effektivitet, säkerhet och nöje hjälper jag dig att nå dina fitnessmål på ett sätt som passar din livsstil.</p>
              </div>
              <div class="col">
                <div> 
                  <font-awesome-icon icon='fa-solid fa-dumbbell' size="l" pull="left"  />
                  <h2> Bygga Muskler</h2>
                  </div>
                  <p>Bygg muskler på ett hållbart sätt med en balans av träning, kost och återhämtning. Som din tränare fokuserar jag på progressiv överbelastning och specifika övningar för att utveckla robust muskelmassa.</p>
                </div>
                <div class="col">
                  <div>
                 <font-awesome-icon icon="fa-solid fa-seedling" size="l" pull="left"   />
                  <h2>Kostråd</h2>
                  </div>
                  <p>Jag erbjuder vetenskapligt baserade kostråd för att förbättra din prestation och återhämtning. Få skräddarsydda måltidsplaner och råd om näringsämnen som kompletterar din träning.</p>
                </div>
            </div>
                
      </div>
  
      <!-- Card for 'Mina utbildningar' -->
      <h2>Mina utbildningar</h2>
          <div class="box"><div class="rectangle"></div></div>
          <div class="certs">
        <img src="../assets/cert_pt.webp" alt="">
        
         

          <img src="../assets/cert_kost.webp" alt="">


          <img src="../assets/cert_kost_träning.webp" alt="">


           


           <img src="../assets/cert_träningsinstruktör.webp" alt="">
           <!--<img class="horis" src="../assets/cert_soma.webp" alt="">-->

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
  .info-cols{
    display:flex;
    justify-content: space-evenly;
    align-items: center;
    flex-wrap: wrap;
    gap:1rem;
    margin-bottom:2rem;
    margin-top:2rem;
  }
  .certs{
    display: flex;
    flex-wrap: wrap;
    gap:1rem;
  }
  .certs img{
    width:250px;
  }
  .info-cols p {
    font-size: 16px;
    padding:0rem 2rem 0rem 2rem;
  }
  .horis{
    transform: rotate(-90deg);
  }
 
  .col div{
    display:flex;
    justify-content: center;
    align-items: center;
    gap:0.5rem;
  }
  .info-cols .col{
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
    width:400px;
  }
  .cards-container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    gap: 1rem;
    justify-content: space-around;
    margin-bottom: 5rem;
  }
  .card h2 {
    font-weight: bold;
  }
  div ul{
    display:flex;
    justify-content: space-evenly;
    margin-top:2rem;
    margin-bottom: 2rem;
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
    padding-bottom:1rem;
  
  }
  .box {
    width: 250px;
    height: 3px;
    background-color: #f1c6b8;
    
    margin-bottom: 20px;
  }
  .card {
    background: #FFFFFF;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.25);
    padding: 40px;
    width: 46%; /* You can adjust the width as needed */
  }
  
  
  
  .card ul {
    list-style: none;
    padding: 10px;
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
  @media (max-width: 800px) {
    .card{
      width:80%;
    }
    .certs{
      justify-content: center;
    }
    
  }
  </style>
  