<template>
  <div v-if="ResumeArray">
    <div v-for="item in ResumeArray" :key="item">
  
      <div id="resume-card" class="container m-0 p-0 mx-auto mt-5 pt-5">
        <div class="row">
          <div class="card bg-transparent">
            <div class="card-body">
              <h4 class="card-title">{{ item.heading }}</h4>
              <p class="card-text">{{ item.year }}</p>
              <img :src="item.image" :style="{width: '300px', height: '250px'}" class="img-thumbnail card-img-top">
              <br>            
              <br>            
              <p class="card-text w-50 mx-auto">{{ item.text }}</p>
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
      ResumeArray: [
        {
          heading: 'Norman Henshilwood High School',
          year: 2016,
          image: 'https://i.postimg.cc/Wzkj8tZf/Polish-20221013-223104571.jpg',
          text: "Attended Secondary School at Norman Henshilwood High School in 2016, Also spent a portion of my time attending Frank Joubert Art School at the same time gaining valuable artistic insight and developing the creative instinct"
        },
        {
          heading: 'Darun Naim',
          year: "2017-2019",
          // image: 'https://i.postimg.cc/vHwhZWvt/DN-Logo-Transparent-e1607643685726.png',
          image: 'https://i.postimg.cc/x85mtdtw/Web-capture-14-1-2023-9959-darun-naim-co-za.jpg',
          // image: 'https://i.postimg.cc/KYrQ5Mzc/image.jpg',
          text: 'Spent 2 years studying Islamic religious studies (Arabic translation and Morphology) at Darun Naim Islamic Institute. Shortly after, i spent some time helping out my Grandmother with her Badge Making business. Beveling of badges, packaging and deliveries to other schools and businesses for over a year while looking to make a career choice.'
        },
        {
          heading: 'Exclusive Badge Company',
          year: "2020",
          image: 'https://i.postimg.cc/TYm1d1Vf/Badge-Making.jpg',
          // image: 'https://i.postimg.cc/KYrQ5Mzc/image.jpg',
          text: 'Spent a year assisting with the beveling of badges, packaging and deliveries to primary and high schools and certain select private businesses nearby'
        },
        {
          heading: 'Sales - Outbound',
          year: '2022',
          image: 'https://i.postimg.cc/435Zmh9W/Polish-20221013-234939489.jpg',
          text: 'Has spent a little time on and off employed in the sales industry providing inbound and outbound services while at home'
        },
        {
          heading: 'Census - STATS SA',
          year: '2022',
          // image: 'https://i.postimg.cc/PqRHWnSD/Polish-20221013-235216197.png',
          // image: 'https://i.postimg.cc/KYrQ5Mzc/image.jpg',
          image: 'https://i.postimg.cc/jdNHpsCJ/Web-capture-14-1-2023-92830-www-fotor-com.jpg',
          text: 'Last employed under StatsSA where time was spent as a fieldworker conducting data collection, data capturing, data processing ,and some supervisory work where communication skills and drive to push forward is necessary, Ive gained valuable experience and perspectives of different types of people from all backgrounds, interviewing and having conversations with thousands of people.'
        },
      ]
    }
  }
}
</script>


<style scoped>
/* #resume-card{
  text-shadow: 4px 4px 4px rgb(0, 0, 0);
} */
.img-thumbnail:hover{
  transform: scale(1.01); 
}
</style>