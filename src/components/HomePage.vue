<template>
  <div id="home">

    <div class="container">

      <div class="row justify-content-evenly mt-5 pt-4 table-fluid text-center position-relative">
        <div class="col-12">
          <!-- <h4>My Portfolio</h4> -->
          <h4>Hello, My Name is Umayr</h4>
          <p> I believe Coding is the future</p>
          <p>I am a student and an aspiring web developer</p>
        </div>

        <div class="row justify-content-evenly table-fluid text-center position-relative">
          <div class="col-12">
            <img src="https://i.postimg.cc/654xP1PF/Profile-image.jpg" class="img-thumbnail" width="300px"
              height="300px" alt="Barcode" loading="lazy">
          </div>
        </div>

        <!--SOCIAL MEDIA POPOVER-->
        <button id="socials-btn" class="btn btn-outline-light mt-2 w-25" type="button" data-bs-toggle="offcanvas"
          data-bs-target="#offcanvasBottom" aria-controls="offcanvasBottom">socials</button>

        <div class="offcanvas offcanvas-bottom" tabindex="-1" id="offcanvasBottom"
          aria-labelledby="offcanvasBottomLabel">

          <div class="offcanvas-header">
            <h5 class="offcanvas-title mx-auto" id="offcanvasBottomLabel">Socials</h5>
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>

          <div class="offcanvas-body mx-auto overflow-hidden">
            <!--overflow-hidden removes the horizontal scroll (bootstrap)-->
            <div>
              <a href="https://www.facebook.com/profile.php?id=100003367218579">
                <div class="SocialIconContainer"></div>
              </a>
              <a href="https://github.com/UmayrNordien">
                <div class="SocialIconContainer2"></div>
              </a>
              <a href="https://www.instagram.com/umayrnordien/">
                <div class="SocialIconContainer3"></div>
              </a>
            </div>
          </div>
        </div>

      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'HomePage',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">

h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}


/* ANIMATION */
.SocialIconContainer {
  /* Shape */
  border: none;
  border-radius: 30px;

  width: 50px;
  height: 50px;
  margin: 15px;
  float: right;

  /* position */
  float: right;

  background-image:url(https://i.postimg.cc/YSXg3j67/output-onlinepngtools.png);
  background-size: cover;
}

.SocialIconContainer2 {
  /* Shape */
  border: none;
  border-radius: 30px;

  width: 50px;
  height: 50px;
  margin: 15px;
  float: right;

  /* position */
  float: right;


  background-image:url(https://i.postimg.cc/SRHHzyT7/output-onlinepngtools-1.png);

  background-size: cover;
}

.SocialIconContainer3 {
  /* Shape */
  border: none;
  border-radius: 30px;

  width: 50px;
  height: 50px;
  margin: 15px;
  float: right;

  /* position */
  float: right;


  background-image:url(https://i.postimg.cc/4xfj7Fw0/output-onlinepngtools-2.png);
  background-size: cover;
}

/* ICON HOVER */
.SocialIconContainer:hover {
  animation: firstanimation 3s infinite;
}

.SocialIconContainer2:hover {
  animation: firstanimation 3s infinite;
}

.SocialIconContainer3:hover {
  animation: firstanimation 3s infinite;
}

@keyframes firstanimation {
  0% {
    background-color: rgb(72, 56, 56);
    transform: translateX(10);

  }

  25% {
    transform: scale(2);
  }

  50% {
    background-color: rgb(66, 133, 91);
    transform: rotate(300deg);
  }

  75% {
    background-color: rgb(144, 183, 125);
    transform: translateX(50);
  }

  100% {
    background-color: rgb(210, 215, 159);
    transform: translateX(50);
  }
}
.btn:hover{
    background-color: #D2D79F;
}

#home{
  margin-top: 85px;
  margin-bottom: 5px;
}

.img-thumbnail:hover{
  transform: scale(1.01); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
// @media screen and (max-width: 767px) {
//     #home{
//       margin-top: 55px;
//       margin-bottom: 75px;
//     }
// }
// @media screen and (max-width: 576px) {
//     #home{
//       margin-top: 75px;
//     }
// }
// @media screen and (max-width: 380px) {
//     #home{
//       margin-top: 22.5px;
//     }
// }

#socials-btn:hover{
  transform: translateY(2px);
  scale: (1.05);
  transition: 2s;
}
</style>
