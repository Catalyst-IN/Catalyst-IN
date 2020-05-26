<template>
  <carousel-3d>
    <slide :index="0" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/anubhav.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          IOS app for catalyst
        </p>
        <div class="centered">Anubhav Singh <br />Admin</div>
      </div>
    </slide>
    <slide :index="1" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/pushpinder.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          IOS app for catalyst
        </p>
        <div class="centered">Pushpinder Pal Singh<br />Admin</div>
      </div>
    </slide>
    <slide :index="2" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/aryaman.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst <br />
          chat bot
        </p>
        <div class="centered">Aryaman Puri <br />Admin</div>
      </div>
    </slide>
    <slide :index="3" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/aashim.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst
        </p>
        <div class="centered">Aashim Garg <br />Mentor</div>
      </div>
    </slide>
    <slide :index="4" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/aman.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst
        </p>
        <div class="centered">Aman Kumar <br />Mentor</div>
      </div>
    </slide>
    <slide :index="5" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/hrishikesh.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst
        </p>
        <div class="centered">Hrishikesh Agarwal <br />Contributor</div>
      </div>
    </slide>
    <slide :index="6" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/vinayak.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst
        </p>
        <div class="centered">Vinayak Sharma <br />Contributor</div>
      </div>
    </slide>
    <slide :index="7" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/bindusar.jpg" />
        <p class="img__description">frontend website catalyst</p>
        <div class="centered">Bindusar Maurya <br />Contributor</div>
      </div>
    </slide>
    <slide :index="8" class="team">
      <div class="img__wrap">
        <img class="img__img" src="../assets/Sapna.jpg" />
        <p class="img__description">
          formal website catalyst <br />
          frontend website catalyst
        </p>
        <div class="centered">Hari Sapna Nair <br />Contributor</div>
      </div>
    </slide>
  </carousel-3d>
</template>

<script>
import { Carousel3d, Slide } from "vue-carousel-3d";
export default {
  components: {
    Carousel3d,
    Slide,
  },
};
</script>

<style scoped>
.team {
  object-fit: fill;
}
img {
  width: 100%;

  object-fit: cover;
}
img:hover {
  opacity: 60%;
}
.centered {
  text-align: center;
  position: absolute;
  top: 90%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-family: "Ubuntu", sans-serif;
  font-size: 16px;
  font-weight: bolder;
  background-color: #ffd633;
  opacity: 80%;
  border-radius: 5px;
}

* {
  margin: 0;
  padding: 0;
  border: 0;
}

.img__description {
  text-align: center;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(255, 214, 51, 0.4);
  font-family: "Ubuntu", sans-serif;
  color: #fff;
  visibility: hidden;
  font-weight: bolder;
  font-size: 24px;
  opacity: 0;
  padding-top: 20%;
  /* transition effect. not necessary */
  transition: opacity 0.2s, visibility 0.2s;
}

.img__wrap:hover .img__description {
  visibility: visible;
  text-align: center;
  opacity: 1;
}
</style>
