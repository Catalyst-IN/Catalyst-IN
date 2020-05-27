<template>
  <div>
      <div class="row">
          <div class="design"> 
                <img src="../assets/color-bar.png" class="footer-img"/>
          </div>
          <div class="slogan col-5">
              <p><span>Young Imagination Network!</span>
                 <br> 
                <a href="#"><button id="donate">DONATE</button></a>
              </p>
              
          </div>
      </div>
      <br>
    <div class="row">
        <div class="col-6 aim">
            <h2>Aim of our organization</h2>
            <p> The aim of the Catalyst network is to provide a platform to all beginner developers to come and work with us on live open source projects; it helps them become experienced contributors as well as skilled developers.

                We also provide a space to all developers who have new, exciting ideas in mind that may open possibilities of discussion in society. As an organisation full of skilled developers we can work with you to help make your ideas reality. </p>
        </div>
        <div class="col-6">
            <img src="../assets/open-source.png" height="100%" width="100%"/>
        </div>
    </div>
  </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    .aim{
        font-family: 'Ubuntu', sans-serif;
        text-align: justify;
        font-size: 18px;
    }
    .aim h2{
        color: black ;
    }
    .aim h2:hover{
        color: black;
    }
    .gif{
        box-shadow: 3px 3px grey;
    }
    .gif:hover{
        box-shadow: 3px 3px #ffd633 ;
    }

    .design img{
        /* width: 80%;
        height: 120px; */
        display: inline-block;
    }

    .slogan{
        display: inline-block;
    }
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
    .slogan p{
        font-size: 30px;
        color: #54BCEB;
        font-family: 'Roboto', sans-serif;
    }

    #donate{
        background-color: rgb(235, 61, 30);
        color: white;
        width: 300px;
        font-weight: bold;
        border-radius: 10px;
        border: 1px solid rgb(235, 61, 30);
    }

    .slogan span{
        color:#8d2165;
         font-size: 30px;
         font-family: 'Roboto', sans-serif;
         font-weight: bold;
    }
</style>
