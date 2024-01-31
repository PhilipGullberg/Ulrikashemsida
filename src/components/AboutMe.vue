<template>

  <div class="card-container">

    <div class="card-content">
        <div class="order">
          <div class="textBox">
            <div class="box"><div class="rectangle"></div></div>
            <h2 class="card-title">Vem är jag?</h2>
            
              <p class="card-text">Jag heter <strong>Ulrika Andersson </strong>och är utbildad PT med över 35 års erfarenhet. För mig är träning en livsstil som ger glädje til vardagen. Jag vill hjälpa andra att hitta det underbara med träningen och få in det i sin vardag. Jag anpassar mina träningsprogram efter just dig.</p>
              <router-link to="/about"><button class="card-button">Läs mer</button></router-link>
          </div>
          <div class="card-image">
            <img src="../assets/IMG_0003.webp" alt="Nature Image">
          </div>
        </div>
   </div>
      <div class="img-card-container">
          <div class="card" style="background-image: url(../src/assets/IMG_1023.webp);"></div>
          <div class="card" style="background-image: url(../src/assets/IMG_2702.webp);"></div>
          <div class="card" style="background-image: url('../src/assets/IMG_0009.webp');"></div>
          
      </div>
  </div>
  <div class="order">  <div class="container-fluid">
      <div class="col-lg-6 col-lg-offset-0 col-md-6 col-md-offset-0 col-sm-10 col-sm-offset-1 col-xs-12">
          <figure>
              <div class="media"></div>
              <figcaption>
               
                  <svg viewBox="0 0 200 200" version="1.1" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
                      <defs>
                        
                          <mask id="mask" x="0" y="0" width="100%" height="100%">
                              <rect id="alpha" x="0" y="0" width="100%" height="100%"></rect>
                              <text class="title" dx="50%" dy="2.5em">NJUT</text>
                              <text class="title" dx="50%" dy="3.5em">AV</text>
                              <text class="title" dx="50%" dy="4.5em">TRÄNING</text>
                          </mask>
                      </defs>
                      <rect id="base" x="0" y="0" width="100%" height="100%"></rect>
                  </svg>
                  <div class="body">
                     <div class="box"><div class="rectangle"></div></div>
                      <p>Träna tillsammans för att skapa glädje, styrka och livsnjutning. Jag hjälper dig att må bättre.</p>
                  </div>
              </figcaption>
              
          </figure>
      </div>      
  </div>

  <div class="container-fluid">
        <div class="col-lg-6 col-lg-offset-0 col-md-6 col-md-offset-0 col-sm-10 col-sm-offset-1 col-xs-12">
            <figure>
                <div class="media" id="image"></div>
                <figcaption>
                  
                    <svg viewBox="0 0 200 200" version="1.1" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
                        <defs>
                          
                            <mask id="second" x="0" y="0" width="100%" height="100%">
                                <rect id="alpha-second" x="0" y="0" width="100%" height="100%"></rect>
                                 <text class="title" dx="50%" dy="2.5em">LÄR</text>
                                <text class="title" dx="50%" dy="3.5em">DIG</text>
                                <text class="title" dx="50%" dy="4.5em">KÄMPA</text>
                            </mask>
                        </defs>
                        <rect id="second-mask" mask="url(#second)" x="0" y="0" width="100%" height="100%"></rect>
                    </svg>
                    <div class="body">
                      <div class="box"><div class="rectangle"></div></div>
                        <p>Jag hjälper dig nå just DINA mål, jag vill att du ska utvecklas efter dina förutsättningar</p>
                    </div>
                </figcaption>
              
            </figure>
        </div>      
    </div>
  </div>
  </template>
  
  <script>
  export default {
    name: 'ProfileSection',
    // component logic
  }
  </script>
  
  <style scoped>
  #image{
    background-image:url(../assets/IMG_0072.webp);
  }
  .img-card-container{
    display:flex;
    justify-content: center;
  }
  .card {
      width: 180px;
      height: 350px;
      background-size: cover;
      background-position: center;
      align-self:center;
      margin-left:-45px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.5);
  }

  .card:nth-child(1) { transform: rotate(-10deg);}
    .card:nth-child(2) { transform: rotate(0deg);
    transform:translate(0px,-10px) }
    .card:nth-child(3) {transform: rotate(10deg);}
    .card:nth-child(4) { top: 60px; left: 60px; }
  body {
     
      margin: 0;
      padding: 0;
      background-color: #ececec;
  }
  .order{
    display:flex;
    
    justify-content: space-around;
  }

  .card-container {
      display:flex;
      flex-wrap: wrap;
      justify-content: space-between;
      
      margin-top:1rem;
      margin-bottom:5rem;
      border-radius: 8px;
  }

 

  .card-image img {
      width: 100%;
      display: block;
      border-radius: 0px 8px 8px 0px;
  }

  .photographer-credit {
      position: absolute;
      bottom: 10px;
      left: 10px;
      font-size: 14px;
      color: white;
      background: rgba(0, 0, 0, 0.5);
      padding: 5px;
 
  }
 .textBox{
  padding:3rem;
  padding-bottom: 1rem;
 }
  .card-content {

      background-color: white;
      width:750px;
      margin-left: 1rem;
      z-index: 1;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      border-radius: 8px;

  }

  .card-title {
      font-size: 2em;
      margin-bottom: 20px;
      margin-top:10px;
     
  }

  .card-text {
      color: #333;
      margin-bottom: 20px;
      
       
  }

  .card-button {
      background-color: #f1c6b8;
      color: black;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-transform: uppercase;
  }

  .card-button:hover {
      background-color: #f9b5a1;
      
  }

  @media (max-width: 900px) {
      .card-container {

          padding: 2rem;
          justify-content: center;
          gap:2rem;
      }
      
      .order{
        justify-content: center;
        flex-direction: column;
      }
      .order img{
        width:60%;
        
      }

      .card-content {
          width: 90%;
            padding: 2rem;
      }

      .card-image {
          position: static;
          margin-top:1rem;
          margin-bottom: 1rem;
          
      }
      .order{
        flex-direction: column;
      }
      .container-fluid{
        width:400px;
      }
  }

  .aboutsection{
    display:flex;
  }
  .arrow{
     transform:rotate(90deg);
  }
  .container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    padding: 20px;
    background: #fff; /* or any color you want */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    margin: 20px;
    border-radius: 8px;
   
   
  }
  .box {
    width: 220px;
    height: 3px;
    background-color: #f1c6b8;
    margin-bottom:1rem;
  }
  
 
  .content {
    flex: 1;
    max-width: 500px;
    align-self: start;
  }
  .content h2{
    font-weight: bold;
  }
  .content p{
    font-size:16px;
  }
  .image-container img {
    flex: 1;
    max-width: 400px;
    height: 300px;
    border-radius: 10px;
  }
  
  @media (max-width: 768px) {
    .container {
      flex-direction: column;
    }
    .card-container{
      padding:0rem;
    }
    .textBox{
      padding:0rem;
    }
  }
  
  .container-fluid {
      text-align: center;
      margin-bottom: 5rem;
      width: 400px;
      padding:2rem;
  }

  .media {
    background-image: url(../assets/IMG_1438.webp);
      background-position: center;
      background-size: cover;
      height: 100%;
      position: absolute;
      transition: all 0.3s ease;
      width: 100%;
      border-radius: 8px;
  }

  figure {
      height: 370px;
      overflow: hidden;
      position: relative;
      border-radius: 8px;
      
  }

  figure a {
      height: 100%;
      left: 0;
      position: absolute;
      top: 0;
      width: 100%;
      z-index: 3;
  }

  figure:hover .media {
      transform: scale(1.25);
      border-radius: 8px;
  }

  figcaption {
      color: #252830;
      height: calc(100% - 30px);
      margin: 15px;
      left: 0;
      position: absolute;
      top: 0;
      width: 250px;
      
  }

  .body {
      background-color: #ffffff;
      bottom: 0;
      padding: 15px;
      position: absolute;
      width: 100%;
  }

  svg {
      height: inherit;
      width: 100%;
      border-radius: 8px;
  }

  svg text {
      text-anchor: middle;
      
  }

  #alpha {
      fill: rgb(255, 255, 255);
      
  }
  #alpha-second{
    fill:white;
  }

  .title {
      font-size: 28px;
      font-family: "Montserrat";
      letter-spacing: 5px;
  }

  #base {
      fill: #ffffff;
      -webkit-mask: url(#mask);
      mask: url(#mask);
  }
  #second-mask {
        fill: #ffffff;
        -webkit-mask: url(#second);
        mask: url(#second);
  }
  .order{
    justify-content: center;
    align-items: center;
  }
  

  </style>
  