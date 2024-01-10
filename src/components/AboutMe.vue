<template>
    <div class="container">
      <div class="content">
        <h2>Vem är jag?</h2>
        <br>
        <p>Jag heter Ulrika Andersson och är utbildad PT med över 35 års erfarenhet. För mig är träning en livsstil som ger glädje til vardagen. Jag vill hjälpa andra att hitta det underbara med träningen och få in det i sin vardag.Mitt motto är att alla kan träna, man måste bara hitta sitt sätt. Det är där jag är duktig på att hjälpa till med. Jag anpassar mina träningsprogram efter just dig.</p>
        <!-- Add more content here -->
      </div>
      <div class="image-container">
        <img src="../assets/muddyullis.png" alt="">
        <!-- Image will be placed as a background in CSS -->
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
  .container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    padding: 20px;
    background: #fff; /* or any color you want */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    margin: 20px;
    gap: 20px;
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
    margin-left:4rem;
    border-radius: 10px;
  }
  
  @media (max-width: 768px) {
    .container {
      flex-direction: column;
    }
  }
  </style>
  