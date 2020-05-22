<template>
    <div class="row">
        <div class="col-6 aim">
            <h2>Aim of our organization</h2>
            <p>  </p>
        </div>
        <div class="col-6">
            <img src="../assets/giphy.gif" width="400" height="240" class="gif"/>
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
    }
    .aim h2{
        color: #ffd633 ;
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
</style>
