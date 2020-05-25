<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div id="root">
            <div class="oval">
                <div class="content">
                    <div class="title">
                        <slot name="title"></slot>
                    </div>
                    <div class="body">
                        <slot name="body"></slot>
                    </div>
                    <div class="link">
                        <slot name="link"></slot>
                    </div>
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
    body {
        font-family: 'Ubuntu', sans-serif;
        text-align: center;
    }
    .oval {
        height: 400px;
        width: 300px;
        background-color: rgb(255, 204, 7);
        border-radius: 50%;
        box-shadow: 4px 4px rgba(24,24,24,0.49);
        transition: width 2s, height 2s;
        transition: all 1s ease-in-out;
    }
    .body{
        margin: 20px 20px 20px 20px;
        font-size: 18px;
        background-color: rgba(255,255,255,0.5);
        border-radius: 15px;
    }
    .title{
        margin: 50px 50px 20px 50px;
        color: white;
        font-size: 16px;
        border-bottom: 1px solid grey;
    }
    .oval:hover{

        height: 340px;
        width: 220px;
    }
</style>