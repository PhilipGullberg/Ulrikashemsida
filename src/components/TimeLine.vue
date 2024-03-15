<template>
<h1>Mina utbildningar och tidigare arbeten</h1>
 
  <div class="center"><h2>Studier</h2>
  <h2>Arbeten</h2></div>
  
 <ul>
    <li class="study">
        <div class="date">2017</div>
        <div class="title">Studerade</div>
        <div class="descr">Soma move instruktörsutbildning</div>
    </li>
    <li class="work">
        <div class="date">2014-2016</div>
        <div class="title">Arbetade</div>
        <div class="descr">Bodypump, Bodybalance och Spinninginstruktör Nordic Wellness, Norrköping</div>
    </li>
    <li class="study">
        <div class="date">2016</div>
        <div class="title">Studerade</div>
        <div class="descr">The Academy, KTK (kost och träningskonsult)</div>
    </li>
    <li class="work">
        <div class="date">1997-2013</div>
        <div class="title">Arbetade</div>
        <div class="descr">Ekonomiansvarig, Halmstad, Aerobic Klubb</div>
    </li>
    <li class="work">
        <div class="date">1996-2000</div>
        <div class="title">Arbetade</div>
        <div class="descr">Friskvårdsinformatör, Landstinget Halland</div>
    </li>
    <li class="study">
        <div class="date">1998-2007</div>
        <div class="title">Studerade</div>
        <div class="descr">
          <ol>
            <li>Tobaksprevention Mälardalens högskola (1998)</li>
            <li>Hogia PA-kompetens AB, Diplomerad personaladministratör (2004)</li>
            <li>Högskolan i Halmstad 5p, ”Personal- och ledarskapsutveckling inom idrottsorganisationer och hälsopromotivt arbete.” (2007)</li>
            <li>Högskolan i Halmstad 5p, ”Det strategiska ledarskapet inom idrottsorganisationer och hälsopromotivt arbete.”</li>
          </ol>
        </div>
    </li>
    <li class="work">
        <div class="date">1986-1990</div>
        <div class="title">Arbetade</div>
        <div class="descr">Undersköterska, Länssjukhuset i Halmstad</div>
    </li>
    <li class="study">
        <div class="date">1985-1987</div>
        <div class="title">Studerade</div>
        <div class="descr">Idrottspedagoglinjen, Högskolan i Halmstad</div>
    </li>
    <li class="work">
        <div class="date">1984-1985</div>
        <div class="title">Arbetade</div>
        <div class="descr">Undersköterska, S:t Eriks sjukhus i Stockholm</div>
    </li>
    <li class="study">
        <div class="date">1981-1983</div>
        <div class="title">Studerade</div>
        <div class="descr">Vårdlinjen på Kvarningeskolan i Jakobsberg</div>
    </li>
</ul>

</template>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap");

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.study{
  
  --accent-color:#f1c6b8;
}

.work{
  --accent-color:#1b88d1;
}
body {
  --color: rgba(30, 30, 30);
  --bgColor: rgba(245, 245, 245);
  min-height: 100vh;
  display: grid;
  align-content: center;
  gap: 2rem;
  padding: 2rem;
  font-family: "Poppins", sans-serif;
  color: var(--color);
  background: var(--bgColor);
}

h1 {
    margin-top: 4rem;
    margin-bottom: 2rem;
  text-align: center;
  font-size:38px;
}


ul{
  --col-gap: 2rem;
  --row-gap: 2rem;
  --line-w: 0.25rem;
  display: grid;
  grid-template-columns: var(--line-w) 1fr;
  grid-auto-columns: max-content;
  column-gap: var(--col-gap);
  list-style: none;
  width: min(70rem, 90%);
  margin-inline: auto;
}

/* line */
ul::before {
  content: "";
  grid-column: 1;
  grid-row: 1 / span 20;
  background: rgb(225, 225, 225);
  border-radius: calc(var(--line-w) / 2);
}

/* columns*/

/* row gaps */
ul li:not(:last-child) {
  margin-bottom: var(--row-gap);
}

/* card */
ul li {
  grid-column: 2;
  --inlineP: 1.5rem;
  margin-inline: var(--inlineP);
  grid-row: span 2;
  display: grid;
  grid-template-rows: min-content min-content min-content;
}

/* date */
ul li .date {
  --dateH: 3rem;
  height: var(--dateH);
  margin-inline: calc(var(--inlineP) * -1);

  text-align: center;
  background-color: var(--accent-color);

  color: white;
  font-size: 1.1rem;
  font-weight: 700;

  display: grid;
  place-content: center;
  position: relative;

  border-radius: calc(var(--dateH) / 2) 0 0 calc(var(--dateH) / 2);
}

/* date flap */
ul li .date::before {
  content: "";
  width: var(--inlineP);
  aspect-ratio: 1;
  background: var(--accent-color);
  background-image: linear-gradient(rgba(0, 0, 0, 0.2) 100%, transparent);
  position: absolute;
  top: 100%;

  clip-path: polygon(0 0, 100% 0, 0 100%);
  right: 0;
}

/* circle */
ul li .date::after {
  content: "";
  position: absolute;
  width: 2rem;
  aspect-ratio: 1;
  background: var(--bgColor);
  border: 0.3rem solid var(--accent-color);
  border-radius: 50%;
  top: 50%;

  transform: translate(50%, -50%);
  right: calc(100% + var(--col-gap) + var(--line-w) / 2);
}
ul li .title{
  font-size: 1.1rem;
  font-style: bold;
}

/* title descr */
ul li .title,
ul li .descr {
  background: var(--bgColor);
  position: relative;
  padding-inline: 1.5rem;
  
}
ul li .title {
  overflow: hidden;
  padding-block-start: 1.5rem;
  padding-block-end: 1rem;
  font-weight: 500;
}
ul li .descr {
  padding-block-end: 1.5rem;
  font-weight: 300;
}

/* shadows */
ul li .title::before,
ul li .descr::before {
  content: "";
  position: absolute;
  width: 90%;
  height: 0.5rem;
  background: rgba(0, 0, 0, 0.5);
  left: 50%;
  border-radius: 50%;
  filter: blur(4px);
  transform: translate(-50%, 50%);
}
ul li .title::before {
  bottom: calc(100% + 0.125rem);
}

ul li .descr::before {
  z-index: -1;
  bottom: 0.25rem;
}
.center{
  display:none
}

@media (min-width: 40rem) {
  .center{
    display:flex;
    justify-content: center;
    gap:30rem;
    margin-bottom:2rem;
  }
  ul {
    grid-template-columns: 1fr var(--line-w) 1fr;
  }
  ul::before {
    grid-column: 2;
  }
  ul li:nth-child(odd) {
    grid-column: 1;
  }
  ul li:nth-child(even) {
    grid-column: 3;
  }

  /* start second card */
  ul li:nth-child(2) {
    grid-row: 2/4;
  }

  ul li:nth-child(odd) .date::before {
    clip-path: polygon(0 0, 100% 0, 100% 100%);
    left: 0;
  }

  ul li:nth-child(odd) .date::after {
    transform: translate(-50%, -50%);
    left: calc(100% + var(--col-gap) + var(--line-w) / 2);
  }
  ul li:nth-child(odd) .date {
    border-radius: 0 calc(var(--dateH) / 2) calc(var(--dateH) / 2) 0;
  }
}

.credits {
  margin-top: 1rem;
  text-align: right;
}
.credits a {
  color: var(--color);
}

h1{
  margin-bottom: 2rem;
}
</style>