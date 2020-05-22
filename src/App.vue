<template>
    <div>
        <div class="container">
            <appheader></appheader>
        </div>
        <hr>
        <div class="container">
            <appaim></appaim>
        </div>
        <hr>
        <div class="container">
            <appfooter></appfooter>
        </div>
    </div>
</template>

<script>
import header from "./components/header";
import footer from "./components/footer";
import aim from "./components/aim";

export default {
    components: {
        appheader: header,
        appfooter: footer,
        appaim: aim
    }
}
</script>

<style>

</style>
