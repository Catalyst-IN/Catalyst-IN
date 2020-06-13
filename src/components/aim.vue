<template>
    <div>
        <div class="row">
            <div class="design">
                <img src="../assets/color-bar.png" class="footer-img" />
            </div>
            <div class="slogan col-lg-5 col-sm-10">
                <p>
                    <span>Young Imagination Network!</span>
                    <br />
                    <a href="#"><button id="donate">DONATE</button></a>
                </p>
            </div>
        </div>
        <br />
        <div class="row">
            <div class="col-12 col-sm-12 col-md-12 col-lg-6 col-xl-6 aim">
                <h2>A little more about Catalyst</h2>
                <br />
                <p>
                    With the aim of increasing the awareness about Open Source
                    and encouraging young developers to contribute to these
                    projects, we, at The Catalyst” provide a platform for young
                    developers to contribute and collaborate on open source
                    projects and gain insights to turn into experienced coders.
                </p>

                <p>
                    The Catalyst is an open space where aspiring developers can
                    come forward with their exciting ideas- to change the world
                    for better- and receive guidance and resources to turn that
                    idea into a reality.
                </p>
            </div>
            <div class="col-12 col-sm-12 col-md-12 col-lg-6 col-xl-6">
                <img
                    src="../assets/open-source.png"
                    height="100%"
                    width="100%"
                />
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.aim {
    font-family: 'Ubuntu', sans-serif;
    text-align: justify;
    font-size: 18px;
}
.aim h2 {
    color: black;
}
.aim h2:hover {
    color: black;
}
.gif {
    box-shadow: 3px 3px grey;
}
.gif:hover {
    box-shadow: 3px 3px #ffd633;
}

.design img {
    /* width: 80%;
        height: 120px; */
    display: inline-block;
}

.slogan {
    display: inline-block;
}
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
.slogan p {
    font-size: 30px;
    color: #54bceb;
    font-family: 'Roboto', sans-serif;
}

#donate {
    background-color: rgb(235, 61, 30);
    color: white;
    width: 390px;
    font-weight: bold;
    border-radius: 10px;
    border: 1px solid rgb(235, 61, 30);
}

.slogan span {
    color: #8d2165;
    font-size: 30px;
    font-family: 'Roboto', sans-serif;
    font-weight: bold;
}

@media (max-width: 1190px) {
    .design img {
        padding-right: 10vw;
    }
}

@media (max-width: 600px) {
    .design img {
        width: 300px;
    }

    #donate {
        width: 150px;
    }

    .slogan span {
        font-size: 15px;
    }
}
</style>
