<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div id="root">
            <div class="box">
                <div class="content">
                    <slot name="title" class="title"></slot>
                    <hr>
                    <slot name="body" class="content"></slot>
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
    #root .box {
        width: 270px;
        height: 350px;
        padding: 2rem;
        border-radius: 4px;
        background: #f8ba26;
        /* box-shadow: 0 3px 5px rgba(0, 0, 0, 0.18); */
        box-shadow: 5px 10px 8px #888888;
        color: white;
        display: flex;
        position: relative;
        flex-direction: colunm;
        transition: all 0.5s ease-in-out;
        border-image-slice: 1;
        overflow: hidden;
        transition: width 2s, height 2s;
    }

   #root .box:hover{
        width: 200px;
        height: 300px;
    }


    #root .box .content {
        /* margin: 20px auto 0 auto; */
    }

    #root .box .content p {
        font-size: 20px;
    }

    #root .box .content * {
        margin-bottom: 40px;
        line-height: 1;
    }
    root .box:hover{

    }
    .title{
        text-align: center;
    }

</style>