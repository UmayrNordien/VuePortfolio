<template>
  <!--div for positioning-->
  <div class="testimonial-carousal">
    <div class="container-fluid" id="container-carousal">
      <div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">

        <div class="carousel-inner">
          <!--ACTIVE-->
          <div class="carousel-item active" data-bs-interval="10000" v-for="test in TestimonialActiveArray"
            :key="test.id">

            <img :src="test.image" class="img-fluid d-block w-25 mx-auto" alt="testimony" loading="lazy">
            <p class="lead text-center text-muted"> {{ test.occupation }}</p>
            <h5 class="text-white text-center mx-auto pt-1"> {{ test.name }}</h5>
            <p class="lead text-center text-light w-50 mx-auto px-0 px-md-5 mb-5 pb-5">{{ test.text }}</p>  <!--mb-5 used to create space between the carousal and the copyright-->
          </div>

          <div class="carousel-item" data-bs-interval="10000" v-for="test in TestimonialArray" 
          :key="test.id">

            <img :src="test.image" class="img-fluid d-block w-25 mx-auto" alt="testimony" loading="lazy">
            <p class="lead text-center text-muted">{{ test.occupation }}</p>
            <h5 class="text-white text-center mx-auto pt-1">{{ test.name }}</h5>
            <p class="lead text-center text-light mx-auto w-50 px-lg-5 mb-5">{{ test.text }}
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
                    name: 'Person 1',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    relation: 'student'
                }
            ],
            TestimonialArray:[
                {
                    name: 'Person 2',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    occupation: 'student'
                },
                {
                    name: 'Person 3',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    occupation: 'student'
                },
                {
                    name: 'Person 4',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    occupation: 'lecturer'
                },
                {
                    name: 'Person 5',
                    image: 'https://i.postimg.cc/wMRg77kg/istockphoto-1152265845-170667a.jpg',
                    text: 'lorem',
                    occupation: 'student'
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
  margin-top: 200px;
  overflow-x: none;
}

/* .container-carousal {
  width: 100vw;
  height: 100vh;
}
.carousel-control-prev, .carousel-control-next {
  width: 150px;
} */

</style>