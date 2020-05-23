<template>
    <div>
        <div class="container">
            <appheader></appheader>
        </div>
        <hr>
        <div class="container">
            <appaim></appaim>
            <hr>
        </div>
        <div class="container">
            <h3>Completed projects</h3>
            <br>
            <cp :details="completedprojects"></cp>
            <br><br>
        </div>
        <hr class="container">
        <div class="container">
            <appfooter></appfooter>
        </div>
    </div>
</template>

<script>
import header from "./components/header";
import footer from "./components/footer";
import aim from "./components/aim";
import gridView from "./components/gridView";

export default {
    data: function(){
        return {
            completedprojects: [
                {title: 'chatbot', body: 'This chatbot helps the police in automating response from citizens'},
                {title: 'sample', body: 'sample text for holding place'}
            ]
        };
    },
    components: {
        appheader: header,
        appfooter: footer,
        appaim: aim,
        cp: gridView
    }
}
</script>

<style scoped>
h3{
    color: #f8ba26;
    font-family: 'Ubuntu', sans-serif;
}
</style>
