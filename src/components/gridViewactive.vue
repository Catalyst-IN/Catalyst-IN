<template>
    <div class="row">
        <app-active v-for="project in info" :key="project.id">
            <h1 slot="title">{{ project.title }}</h1>
            <p slot="body">{{ project.body }}</p>
        </app-active>
    </div>
</template>

<script>
    import activeProjects    from "./activeProjects";
    export default {
        props: ['info'],
        components: {
            appActive: activeProjects
        }
    }
</script>

<style>

</style>