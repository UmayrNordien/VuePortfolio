<template>
  <!--div for positioning-->
  <div id="testimonial-carousal" class="testimonial-carousal">
    <div class="container-fluid" id="container-carousal">
      <div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">

        <div class="carousel-inner">
          <!--ACTIVE-->
          <div class="carousel-item active" data-bs-interval="10000" v-for="test in TestimonialActiveArray"
            :key="test.id">

            <img :src="test.image" class="img-fluid d-block w-25 mx-auto" alt="testimony" loading="lazy">
            <p class="lead text-center"> {{ test.occupation }}</p>
            <h5 class="text-white text-center mx-auto pt-1"> {{ test.name }}</h5>
            <p class="lead text-center  w-50 mx-auto px-0 px-md-5 mb-5 pb-5">{{ test.text }}</p>  <!--mb-5 used to create space between the carousal and the copyright-->
          </div>

          <div class="carousel-item" data-bs-interval="10000" v-for="test in TestimonialArray" 
          :key="test.id">

            <img :src="test.image" class="img-fluid d-block w-25 mx-auto" alt="testimony" loading="lazy">
            <p class="lead text-center">{{ test.occupation }}</p>
            <h5 class="text-white text-center mx-auto pt-1">{{ test.name }}</h5>
            <p class="lead text-center mx-auto w-50 px-lg-5 mb-5">{{ test.text }}
            </p>
          </div>

        </div>
        <!--CONTROL BUTTONS-->
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>

      </div>
    </div>
  </div>

</template>


<script>
export default {
    data() {
        return {
            TestimonialActiveArray: [
                {
                    name: 'Javier Goodall',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'He is still a very dedicated and passionate about web development,where he spends a lot of his time completing projects and upskilling himself',
                    occupation: 'student'
                }
            ],
            TestimonialArray:[
                {
                    name: 'Deno Rautenbach',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'Umayrs quiet demeanor creates a mystique aura of wonder around the depth of his character, So deep that all i have for him is the utmost respect and admiration in his stoic approach to life .Having worked with him, I can proudly say his steadfast, results oriented methodology is one everyone should strive for and implement',
                    occupation: 'student'
                  },
                {
                    name: 'Asandile Langeni',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'Umayr is a good person who is quiet but pays attention to everything that is happening around him.He likes to upskill himself so that he can new knowledge all the time.He is always there to lend a helping hand',
                    occupation: 'student'
                },
                {
                    name: 'Aneeqah Brown',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'Umayr is a highly thought intellectual from my perspective. He is not only hardworking but ambitious to recreate his vision exactly as thought of. He does his work accordingly and always provide a helping hand. He has great communication and leadership skills that a company needs especially his creativity',
                    occupation: 'student'
                },
                {
                    name: 'Joel Mukanya',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'Umayr is a very creative, go-getter, and well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I will be very delighted to see him get hired',
                    occupation: 'lecturer'
                },
                {
                    name: 'Person 6',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    occupation: 'student'
                }
            ]
        }
    }
}
</script>


<style scoped>
.testimonial-carousal {
  background-color: none;
  margin-top: 125px;
  overflow-x: none;
}
/* #testimonial-carousal {
  text-shadow: 4px 4px 4px rgb(0, 0, 0);
} */
.img-fluid:hover{
  transform: scale(1.115); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
</style>