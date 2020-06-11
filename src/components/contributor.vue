<template>
    <carousel-3d>
        <slide :index="0" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/anubhav.jpg" />
                <p class="img__description">
                    <br />
                    <span class="centered">
                        Anubhav Singh <br />Admin <br />
                        ios developer(GSoC'20 @amahi)</span
                    >
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/anubhav-singh-27512a167/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/anubhavsingh16"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="1" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/pushpinder.jpg" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered"> Pushpinder Pal <br />Admin</span>
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/pushpinderpalsingh/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/pushpinderpalsingh"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                        <a
                            href="https://technicalnow.in/"
                            alt="Blog"
                            target="_blank"
                            ><i
                                class="fa fa-pencil-square-o"
                                aria-hidden="true"
                            ></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="2" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/arnav.png" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered">Arnav Balyan <br />ML Mentor</span>
                    <br />
                    <span class="social-icons">
                        <a href="" alt="linkedin" target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/ArnavBalyan"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="3" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/aashim.jpg" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered"> Aashim Garg <br />Mentor</span>
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/aashim-garg-370104198/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/aashimgarg"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="4" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/aman.jpg" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered"> Aman Kumar <br />Mentor</span>
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/aman-kumar-6b31b9127/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/Amankumar29"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="5" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/hrishikesh.jpg" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered">
                        Hrishikesh Agarwal <br />Member</span
                    >
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/hrishikesh-agarwal-794801195/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/codetheorem"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
        <slide :index="6" class="team">
            <div class="img__wrap">
                <img class="img__img" src="../assets/vinayak.jpg" />
                <p class="img__description">
                    <br /><br />
                    <span class="centered"> Vinayak Sharma <br />Member</span>
                    <br />
                    <span class="social-icons">
                        <a
                            href="https://www.linkedin.com/in/vinayak-sharma-141096193/"
                            alt="linkedin"
                            target="_blank"
                            ><i class="fab fa-linkedin"></i
                        ></a>
                        <a
                            href="https://github.com/vinayaksh42"
                            alt="github"
                            target="_blank"
                            ><i class="fab fa-github-square"></i
                        ></a>
                    </span>
                </p>
            </div>
        </slide>
    </carousel-3d>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d';
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
    color: black;
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
    font-family: 'Ubuntu', sans-serif;
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

.social-icons a i {
    padding: 10px;
    color: rgb(75, 73, 73);
}
</style>
