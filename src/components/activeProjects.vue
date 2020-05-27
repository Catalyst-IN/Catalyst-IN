<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div id="root">
            <div class="box" >
                <div class="content" >
                    <slot name="image"></slot>
                    <slot name="title" class="title" ></slot>
                    <slot name="subtitle"></slot>
                    <hr>
                    <slot name="body" class="content"></slot>
                    <br>
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

</style>