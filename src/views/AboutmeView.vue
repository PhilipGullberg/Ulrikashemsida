<template>
    
    <div class="intro">
        <div class="left">
            <h2>Ulrika Andersson</h2>
            <p>Hej! Jag är en personlig tränare med många års erfarenhet. För mig är träning en livsstil som ger glädje til vardagen. Jag vill hjälpa andra att hitta det underbara med träningen och få in det i sin vardag. Jag anpassar mina träningsprogram efter just dig.
            </p>
            <br>
            <h2>Mina ledord</h2>
            <ul>
                <li>Stryka i själen</li>
                <li>Glädje i träning</li>
                <li>Alla kan träna</li>
            </ul>
            <br>
            <h2>Mina Certifieringar</h2>
            <br>
            
          <div class="certs">
        <img src="../assets/cert_pt.webp" alt="">
        
         

          <img src="../assets/cert_kost.webp" alt="">


          <img src="../assets/cert_kost_träning.webp" alt="">


           


           <img src="../assets/cert_träningsinstruktör.webp" alt="">
           <!--<img class="horis" src="../assets/cert_soma.webp" alt="">-->

     </div>
        </div>
          
        <div class="right">
            <img src="../assets/ulrikaProf.png" alt="">
        </div>
    </div>
    <Timeline />
</template>
<script>
import Timeline from '../components/TimeLine.vue';

export default {
    name: 'aboutme',
    components: {
        // Register the component
        Timeline
    }
    // component logic
}
</script>
<style>
.box {
    width: 220px;
    height: 3px;
    background-color: #f1c6b8;
    margin-bottom:1rem;
  }
.certs{
    display: flex;
    flex-wrap: wrap;
    gap:1rem;
  }
  .certs img{
    width:150px;
  }
.intro{
    margin-top: 3rem;
    display: flex;
    gap:2rem;
    justify-content: center;
}
.left{
    width:65%;
    padding:0rem 5rem;

}
.left p{
    font-size: 1.1rem;
    margin-top: 1rem;
}
.left ul li{
    font-size: 1.1rem;
}
.right img{
    width:350px;
}
@media screen and (max-width:900px) {
    .intro{
        flex-direction: column;
        align-items: center;
        gap:2rem;
    }
    .left{
        padding:0rem 2rem;
    }
    
}
</style>