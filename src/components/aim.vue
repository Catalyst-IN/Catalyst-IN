<template>
    <div class="row">
        <div class="col-6 aim">
            <h2>Aim of our organization</h2>
            <p>our website provides a comprehensive list of open source events and hackathons that our happening around the world.
                They are listed down in a proper month wise timeline so the user does not face difficulty while searching through the open source events.
                Most of the times students want to participate in the events but they dont know the dates or the event details.
                This repo contains links of the events and when are the events going to take place.</p>
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