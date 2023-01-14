<template>
  <div id="about">

    <div class="row justify-content-evenly position-relative mb-1">
      <div class="col-12">
        <img src="https://i.postimg.cc/W1rTqdhb/Profile-Img2-Blur.jpg"
          class="img-thumbnail image-fluid bg-image hover-zoom" width="300px" height="300px" alt="BlurEffectProfileImg"
          loading="lazy">
      </div>
    </div>

    <div class="row flipcardrow slide">
      <div class="column">
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <span>My name is Umayr Nordien, I was born in Cape Town, Western Cape.
                My hobbies include training and sparring in various Martials Arts including Judo (where I competed
                actively
                throughout High School as regional champion for Western Cape and Boland), Silat and recently Muay Thai.
                I
                believe heavily in discipline and moral values.
                I am also a avid gamer and really enjoy the competitive aspect too
                <br>
                <br>
                <i class="bi bi-arrow-down-circle"></i>
              </span>
            </div>
            <div class="flip-card-back">
              <span>I graduated at Norman Henshilwood High School and studied religious studies thereafter.
                Since, I've gained valuable work experience as a salesman doing both inbound and outbound calls while at
                home.
                I've also been employed at StatsSA, conducting the CENSUS 2022 which has been extremely crucial in my
                overall
                ability
                I was previously interested in animation and graphical design, to seek a career the creative industry.

                These industries are heavily influenced by current technology and trends
                I've chosen to gain programming and coding knowledge to up my skills and to seek employment in the
                computing
                or
                creative space
                I believe coding and programming is the <strong>future</strong></span>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>
#about {
  margin-top: 60px;
  margin-bottom: 25px;
  /* text-shadow: 4px 4px 4px rgb(0, 0, 0); */
}

.slide {
  animation: slidein 1.5s ease 0s 1 forwards;
}

@keyframes slidein {
  from {
    transform: translateY(1244px);
  }

  to {
    transform: translateY(10px);
  }
}

/* RESPONSIVENESS */
@media screen and (max-width: 566px) {
  #about {
    margin-top: 55px;
  }
}

@media screen and (max-width: 380px) {
  #about {
    margin-top: 22.5px;
  }
}

/* FLIPCARD */
div {
  color: white !important;
}

.flipcardrow {
  margin-right: auto !important;
  margin-left: auto !important;
}

.flip-card {
  background-color: transparent;
  width: 600px;
  height: 280px;
  border: 2px solid white;
  border-radius: 20px;
  perspective: 1000px;
  margin: auto;
  margin-bottom: 20px;
}

/* This container is needed to position the front and back side */
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 3s;
  transform-style: preserve-3d;
}

/* Do an horizontal flip when you move the mouse over the flip box container */
.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

/* Position the front and back side */
.flip-card-front,
.flip-card-back {
  position: absolute;
  font-size: 16px;
  height: 100%;
  width: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

/* Style the front side (fallback if image is missing) */
.flip-card-front {
  padding-top: 40px;
  background-color: transparent;
  border-radius: 20px;
  opacity: 75%;
  color: rgb(255, 255, 255);
}

/* Style the back side */
.flip-card-back {
  padding-top: 20px;
  background-color: transparent;
  border-radius: 20px;
  color: rgb(255, 255, 255);
  transform: rotateY(180deg);
}

span {
  line-height: 1px;
}

@media screen and (max-width: 634px) {
  .flip-card {
    width: 450px;
  }
}

@media screen and (max-width: 486px) {
  .flip-card {
    width: 300px;
  }

  .flip-card-front,
  .flip-card-back {
    font-size: 12px;
  }

  .flip-card-front {
    padding-top: 50px;
  }

  .flip-card-back {
    padding-top: 5px;
    padding-right: 5px;
    padding-left: 5px;
  }
}

@media screen and (max-width: 322px) {
  .flip-card {
    width: 280px;
  }

  .img-thumbnail {
    width: 280px;
  }
}

.hover-zoom:hover {
  transform: scale(1.01);
  /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
</style>
