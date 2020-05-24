<template>
    <div class="row">
        <app-quote v-for="project in details" :key="project.id" >
            <h1 slot="title">{{ project.title }}</h1>
            <p slot="body">{{ project.body }}</p>
            <button class="btn btn-info" slot="link"><a :href="project.link" target="_blank">Know More</a></button>
        </app-quote>
    </div>
</template>

<script>
    import completedProjects from "./completedProjects";
    export default {
        props: ['details'],
        components: {
            appQuote: completedProjects
        }
    }
</script>

<style scoped>
.btn{
    background-color: black;
    color: white;
}
</style>