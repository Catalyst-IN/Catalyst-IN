<template>
  <div class="row">
    <app-active v-for="project in info" :key="project.id">
      <h5 slot="title">{{ project.title }}</h5>
      <p slot="body">{{ project.body }}</p>
      <button class="btn btn-info" slot="link">
        <a :href="project.link" target="_blank">Know More</a>
      </button>
      <ul slot="list" style="font-size: 17px;">
        <li v-for="name in project.contri" :key="name.id">{{ name }}</li>
      </ul>
    </app-active>
  </div>
</template>

<script>
import activeProjects from "./activeProjects";
export default {
  props: ["info"],
  components: {
    appActive: activeProjects,
  },
};
</script>

<style></style>
