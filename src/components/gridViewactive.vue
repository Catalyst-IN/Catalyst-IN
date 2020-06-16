<template>
    <div class="row">
        <app-active v-for="project in info" :key="project.id">
            <img
                :src="require('../assets/' + project.imageLink)"
                class="card-img-top"
                slot="image"
                width="320"
                height="190"
            />
            <h5 slot="title">{{ project.title }}</h5>
            <h6 slot="subtitle">{{ project.subtitle }}</h6>

            <div slot="body">
                <span v-if="!project.readMoreActivated"
                    >{{ project.body.slice(0, 50) }}
                </span>
                <a
                    class=""
                    v-if="!project.readMoreActivated"
                    @click="
                        project.readMoreActivated = !project.readMoreActivated
                    "
                    href="#/"
                >
                    Read more...
                </a>
                <span
                    v-if="project.readMoreActivated"
                    v-html="project.body"
                ></span>
            </div>

            <!--      <p slot="body">{{ project.body }}</p>-->
            <button class="btn btn-info" slot="link">
                <a :href="project.link" target="_blank">Know More</a>
            </button>
        </app-active>
    </div>
</template>

<script>
import activeProjects from './activeProjects';
export default {
    name: 'Readmore',
    props: ['info'],
    components: {
        appActive: activeProjects,
    },
};
</script>

<style scoped>
.card-img-top {
    padding-bottom: 20px;
}
h6 {
    color: #8d2166;
}
h5 {
    color: #ec8e2a;
}
button a {
    color: white;
}

button a:hover {
    text-decoration: none;
}
</style>
