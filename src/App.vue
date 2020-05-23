<template>
    <div>
        <div class="container">
            <appheader></appheader>
        </div>
        <hr>
        <div class="container">
            <appaim></appaim>
            <hr>
        </div>>
        <div class="container">
            <h3>Active projects</h3>
            <br>
            <appactive :info="activeprojects"></appactive>
            <br><br>
        </div>
        <hr class="container">
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
import gridViewactive from "./components/gridViewactive";

export default {
    data: function(){
        return {
            completedprojects: [
                {title: 'chatbot', body: 'This chatbot helps the police in automating response from citizens'},
                {title: 'sample', body: 'sample text for holding place'},
                {title: 'sample', body: 'sample text for holding place'},
                {title: 'sample', body: 'sample text for holding place'}
            ],
            activeprojects: [{title: 'Test', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud '},
                {title: 'Test', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation '},
                {title: 'Test', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation '},
                {title: 'Test', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation'}
            ]
        };
    },
    components: {
        appheader: header,
        appfooter: footer,
        appaim: aim,
        cp: gridView,
        appactive: gridViewactive
    }
}
</script>

<style scoped>
h3{
    color: black;
    font-family: 'Ubuntu', sans-serif;
}
</style>
