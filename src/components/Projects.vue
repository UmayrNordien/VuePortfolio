<template>
  <div v-if="ProjectsArray">
    <div v-for="project in ProjectsArray" :key="project">

      <div id="project-card" class="container mx-auto mt-5 pt-5">
        <div class="row">
          <div class="card bg-transparent">
            <div class="card-body">
              <h4 class="card-title">{{ project.heading }}</h4>
              <p class="card-text">{{ project.date }}</p>
              <img :src="project.image" class="card-img-top" alt="">
              <a :href="project.github" id="btn1" class="btn btn-outline-light mt-2 me-5" role="button">Github</a>
              <a :href="project.netlify" id="btn2" class="btn btn-outline-light mt-2 gap-5" role="button">Netlify</a>
            </div>
          </div>
        </div>
      </div>
      
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      ProjectsArray: [
        {
          heading: 'E-Commerce Page',
          date: 'Oct 28, 2022',
          text: '',
          image: 'https://i.postimg.cc/q7GjTWDQ/Ecommerce-Img.png',
          github: 'https://github.com/UmayrNordien/Mock-E-Commerce-Store.git',
          netlify: 'https://mockecommercestore.netlify.app/'
        },
        {
          heading: 'JavaScript E-Commerce Page',
          date: 'Dec 10, 2022',
          text: '',
          image: 'https://i.postimg.cc/jjX0FgHY/seshpos-ecoommerce.png',
          github: 'https://github.com/UmayrNordien/Point-Of-Sale-System-SeshStore',
          netlify: 'https://seshstore-pos.netlify.app/'
        },
        {
          heading: 'Bootstrap Portfolio',
          date: 'Nov 5, 2022',
          text: '',
          image: 'https://i.postimg.cc/nLzbNK0s/Bootstrap-Portfolio.png',
          github: 'https://github.com/UmayrNordien/Bootstrap_Portfolio.git',
          netlify: 'https://umayrnordiensportfolio.netlify.app/'
        },
        {
          heading: 'Calculator',
          date: 'Nov 26, 2022',
          text: '',
          image: 'https://i.postimg.cc/xTcmjB8g/CAL-aesthetic-calculator.png',
          github: 'https://github.com/UmayrNordien/CAL-aesthetic-Calculator.git',
          netlify: 'https://calaestheticcalculator.netlify.app/'
        }
      ]
    }
  }
}
</script>

<style scoped>
#btn1:hover{
  background-color: rgb(144, 183, 125);
}
#btn2:hover{
  background-color: rgb(210, 215, 159);
}
/* #project-card{
  text-shadow: 4px 4px 4px rgb(0, 0, 0);
} */
.card-img-top:hover{
  transform: scale(1.01); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
.btn:hover{
  transform: translateY(2px);
  scale: (1.05);
  transition: 2s;
}
</style>
