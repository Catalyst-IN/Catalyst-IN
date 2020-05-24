<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div id="root">
            <div class="parallelogram">
                <div class="content">
                    <slot name="title" class="title"></slot>
                    <slot name="body" class="content"></slot>
                    <slot name="link"></slot>
                </div>
            </div>
        </div>
    </div>


</template>

<script>
    export default {
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,400;0,700;0,900;1,400&display=swap');

    * {
        margin: 0;
        padding: 0;
        outline: 0;
        box-sizing: border-box;
    }

    html,
    body,
    #root {
        height: 100%;
    }

    #root {
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }
    body {
        font-family: 'Ubuntu', sans-serif;
    }
    #root .parallelogram {
        width: 270px;
        height: 450px;
        padding: 2rem;
        margin: 20px 20px 20px 20px;
        transform: skewY(-10deg);
        border-radius: 4px;
        background: #f8ba26;
        box-shadow: 0 3px 5px rgba(0, 0, 0, 0.18);
        color: white;
        display: flex;
        position: relative;
        flex-direction: colunm;
        transition: all 0.5s ease-in-out;
        border: 4px solid transparent;
        border-image: linear-gradient(30deg, lightgrey 10%, lightyellow 25%, grey 50%, white 75%, black 90%);
        -webkit-border-image: -webkit-linear-gradient(30deg, lightgrey 10%, 	black 25%, lightblue 50%, lightyellow 75%, grey 90%);
        border-image-slice: 1;
    }


    #root .parallelogram .content {
        transform: skewY(10deg);
        margin: 30px auto 0 auto;
    }

    #root .parallelogram .content p {
        font-size: 20px;
    }

    #root .parallelogram .content * {
        margin-bottom: 40px;
        line-height: 1.5;
    }
      #root .parallelogram:hover{
        height: 550px;

    }
    .title{
        text-align: center;
    }

</style>