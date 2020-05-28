<template>
  <div>
    <!--    navbar/header-->

    <div class="container">
      <appheader
        :selected="selected"
        @namewasreset="selected = $event"
      ></appheader>
    </div>
    <hr class="navdivider" />

    <!--    dyanamic components-->

    <keep-alive>
      <component :is="selected"></component>
    </keep-alive>

    <!--    footer-->

    <hr />
    <div class="container">
      <appfooter
        :selected="selected"
        @namewasreset="selected = $event"
      ></appfooter>
    </div>
  </div>
</template>

<script>
import header from "./components/header";
import footer from "./components/footer";
import home from "./home";
import whoweare from "./whoweare";
import whatwedo from "./whatwedo";
import Events from "./Events";
import contact from "./components/contact";
import privacy from "./components/privacy";
import terms from "./components/terms";
import newsletter from "./components/newsletter";

export default {
  data: function () {
    return {
      selected: "home",
    };
  },
  components: {
    appheader: header,
    appfooter: footer,
    home: home,
    whoweare: whoweare,
    whatwedo: whatwedo,
    events: Events,
    contact: contact,
    privacy: privacy,
    terms: terms,
    newsletter: newsletter,
  },
};
</script>

<style scoped>
h3 {
  color: black;
  font-family: "Ubuntu", sans-serif;
}

.navdivider {
  margin-top: 1rem;
}
</style>
