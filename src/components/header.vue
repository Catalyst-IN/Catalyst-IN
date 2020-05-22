<template>
    <nav class="navbar navbar-expand-lg navbar-light header">
        <img src="../assets/logo.png" class="img-thumbnail logo" width="200" height="200">

        <div class="collapse navbar-collapse" id="navbarText">
            <ul class="navbar-nav mr-auto">
            </ul>
            <span class="navbar-text">
                <ul id="icons">
                    <li><img src="../../public/iconfinder_1_Whatsapp2_colored_svg_5296520.png" height="40px" width="40px"/></li>
                    <li><img src="../../public/iconfinder_1_Twitter_colored_svg_5296514.png" height="40px" width="40px"/></li>
                    <li><img src="../../public/iconfinder_1_Linkedin_unofficial_colored_svg_5296501.png" height="40px" width="40px"/></li>
                    <li><img src="../../public/iconfinder_1_Instagram_colored_svg_1_5296765.png" height="40px" width="40px"/></li>
                    <li><img src="../../public/iconfinder_1_Facebook_colored_svg_copy_5296499.png" height="40px" width="40px"/></li>
                </ul>
            </span>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "header"
    }
</script>

<style scoped>
.logo{
    margin: 10px;
}
    .header{
        padding: 20px;
        position: relative;
        border-bottom: 2px solid yellow;
    }
    #icons li{
        display: inline;
        list-style-type: none;
        padding-right: 20px;
        float: right;
    }


</style>