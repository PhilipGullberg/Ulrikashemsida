<template>
    <!--<div class="image-grid">
        <div class="image-item "><img src="../assets/IMG_3401.png" alt="Large Image"></div>
        <div class="image-item"><img src="../assets/IMG_1496.png" alt="Tall Image"></div>
        <div class="image-item wide"><img src="../assets/IMG_0006.png" alt="Image 2"></div>
        <div class="image-item wide"><img src="../assets/IMG_0072.png" alt="Wide Image"></div>
        <div class="image-item wide"><img src="../assets/IMG_1438.png" alt="Large Image"></div>
        <div class="image-item"><img src="../assets/IMG_2702.png" alt="Image 3"></div>
        <div class="image-item"><img src="../assets/IMG_1818.png" alt="Image 4"></div>
        <div class="image-item"><img src="../assets/IMG_1023.png" alt="Image 1"></div>
        <div class="image-item "><img src="../assets/IMG_0003.png" alt="Image 1"></div>
        
      </div>
    -->
</template>
<style>
.image-grid {
    display: grid;
    grid-template-columns: repeat(6, 0.5fr); /* This creates four columns */
    grid-auto-rows: minmax(100px, auto); /* This sets a minimum and maximum row size */
    gap: 5px; /* This adds space between items */
  }
  
  .image-item {
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .image-item img {
    width: 100%;
    height: auto;
    display: block;
  }
  
  /* Specific styles for different image sizes */
  .image-item.large { grid-column: span 2; grid-row: span 2; } /* Large image will take up twice the space */
  .image-item.wide { grid-column: span 2; } /* Wide image will take up two columns but one row */
  .image-item.tall { grid-row: span 2; } /* Tall image will take up two rows but one column */
  
  @media (max-width: 768px) {
    .image-grid {
      grid-template-columns: repeat(2, 1fr); /* On smaller screens, reduce the number of columns to 2 */
    }
  
    .image-item.large, .image-item.wide, .image-item.tall {
      grid-column: span 2; /* All special-sized images will span across all columns on smaller screens */
    }
  }
  </style>
<script>
  export default {
    name: 'ImageGrid',
    // component logic
  }
</script>