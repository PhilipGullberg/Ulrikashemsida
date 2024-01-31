<template>
     <h1>Vad säger andra?</h1>
     <div class="box"><div class="rectangle"></div></div>
      <div class="testimonials-container">
            <!-- Testimonial Card 1 -->
            <div class="testimonial-card">
                <div class="quote">
                    <p>"Jag trodde aldrig att jag skulle se fram emot att gå till gymmet, men det var innan jag började träna med Ulrika. Hennes energi är smittsam och hennes kunskap är omfattande. Hon pushar mig till mina gränser och har lärt mig så mycket om vad min kropp kan göra. Tack vare henne har jag blivit starkare och mer självsäker än jag någonsin varit."</p>
                </div>
                <div class="star">
                 <span style='font-size:2rem;'>&#9733;</span>
                 <span style='font-size:2rem;'>&#9733;</span>
                 <span style='font-size:2rem;'>&#9733;</span>
                 <span style='font-size:2rem;'>&#9733;</span>
                 <span style='font-size:2rem;'>&#9733;</span>
                 </div>
                <img src="https://i.pravatar.cc/300?u=1" alt="Pelican Steve" class="avatar">
                <div class="client-info">
                    <strong>Jennifer Andersson</strong>
                   
                </div>
            </div>
            <div class="testimonial-card">
                    <div class="quote">
                        <p>"Ulrika har en unik förmåga att se exakt vad jag behöver för att lyckas med mina fitnessmål. Hon kombinerar styrka och kondition med en djup förståelse för hur motivation fungerar. Hennes träningspass är utmanande, men alltid anpassade och roliga - en perfekt mix! Tack vare Ulrika ser jag fram emot varje pass med ny energi och entusiasm."</p>
                    </div>
                    <div class="star">
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     </div>
                    <img src="https://i.pravatar.cc/300?u=2" alt="Pelican Steve" class="avatar">
                    <div class="client-info">
                        <strong>Göran Persson</strong>
                       
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="quote">
                        <p>"Som PT överträffar Ulrika alla förväntningar. Hennes personliga träningsprogram har inte bara förändrat min kropp utan också mitt sätt att tänka kring hälsa och träning. Hennes stöd och vägledning har hjälpt mig att uppnå mål jag inte trodde var möjliga. Hon är mer än en tränare; hon är en livsförändrare."</p>
                    </div>
                    <div class="star">
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     <span style='font-size:2rem;'>&#9733;</span>
                     </div>
                    <img src="https://i.pravatar.cc/300?u=3" alt="Pelican Steve" class="avatar">
                    <div class="client-info">
                        <strong>Amy Wong</strong>
                        
                    </div>
                </div>
            <!-- Repeat for other cards -->
        </div>
        
</template>
<style scoped>

.testimonials-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    margin-top:1rem;
    margin-bottom: 7rem;
}
.star{
    display: flex;
    justify-content: center;
}
  .box {
    width: 300px;
    height: 3px;
    background-color: #f1c6b8;
    margin-bottom:1rem;
  }

.testimonial-card {
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    margin: 10px;
    padding: 20px;
    position: relative;
    width: 400px;
}

.quote {
    position: relative;
    background: white;
    border-radius: 5px;
    padding: 20px;
    margin-bottom: 10px;
}

.quote::before {
    content: '';
    width: 0;
    height: 0;
    border-left: 15px solid transparent;
    border-right: 15px solid transparent;
    border-top: 15px solid white;
    position: absolute;
    bottom: -15px;
    left: 50%;
    transform: translateX(-50%);
}

.avatar {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    margin-bottom: 10px;
    position: absolute;
    bottom: -30px;
    left: 50%;
    transform: translateX(-50%);
    border: 3px solid white;
}

.client-info {
    text-align: center;
    margin-top: 40px; /* Space for the avatar */
}

.client-info strong {
    display: block;
    font-size: 0.9em;
    margin-bottom: 1rem;
}

.client-info span {
    font-size: 0.8em;
    color: #555;
}
</style>
<script>
export default {
    name: 'Testimony',
    // component logic
}
</script>