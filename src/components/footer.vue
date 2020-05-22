<template>
    <div>
        <footer class="page-footer">
            <div class="footer-content  flexdisplay">
                <div class="fc-left">
                    <img src="../assets/logo.png"  width="300" height="200">
                </div>
                <div class="fc-right">
                    <div class="fc-nav">
                        <ul>
                            <li><a href="#">PRIVACY POLICY</a></li>
                            <li><a href="#">TERMS OF USE</a></li>
                            <li><a href="#">SUBSCRIBE TO THE NEWSLETTER</a></li>
                            <li><a href="#">CONTACT US</a></li>
                        </ul>
                    </div>
                    <div class="fc-mission">
                        <p>We connect, inspire and guide youth in computing and organizations that view technology 
                        innovation as a strategic imperative.</p>
                        <p>Youth transform technology. </p>
                    </div>
            </div>
            </div>
            <div class="footer-copyright text-center py-3">&copy; Catalyst 2020
                <img src="https://anitab.org/wp-content/assets/images/footer_bars.png" class="footer-img"/>
            </div>
        </footer>
    </div>
</template>

<script>
    export default {
        name: "footer"
    }
</script>

<style scoped>
.footer-img{
    max-width: 100%;
}

.flexdisplay{
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    margin-top: 5%;
}

.fc-right{
    width:50%;
}

.fc-left{
    width: 50%;
    padding-left: 10%;
}


ul{
    list-style-type: none;
}

li{
    margin-top: 2%;
}
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
a,a:visited{
    text-decoration: none;
    text-transform: uppercase;
    font-family: 'Montserrat';
    font-size: 24px;
    font-weight: bold;
    color: #54BCEB;
}

a:hover{
    color: rgb(3, 3, 63);
}

.fc-mission{
    margin-top: 10%;
    font-style: normal;
    font-weight: bold;
    text-align: left;
    line-height: 2;
    font-size: 16px;
    letter-spacing: 0.05em;
    color : #575757;
}


</style>