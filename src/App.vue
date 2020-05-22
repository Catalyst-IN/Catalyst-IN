<template>
    <div>
        <div class="container">
            <appheader></appheader>
        </div>
        <hr class="container">
        <div class="container">
            <appbody></appbody>
            <appbody></appbody>
            <appbody></appbody>
            <appbody></appbody>
        </div>
        <hr class="container">
        <div class="container">
            <appfooter></appfooter>
        </div>
    </div>
</template>

<script>
import header from "./components/header";
import body from "./components/body";
import footer from "./components/footer";

export default {
    components: {
        appheader: header,
        appbody: body,
        appfooter: footer
    }
}
</script>

<style>

</style>
