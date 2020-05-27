<template>
  <div>
    <div class="container">
      <appheader></appheader>
    </div>
    <hr class="navdivider" />
    <div class="container">
      <appaim></appaim>
      <hr />
    </div>
    <div class="container">
      <h3>Events</h3>
      <br />
      <appevents></appevents>
    </div>
    <hr class="container" />
    <div class="container">
      <h3>Active projects</h3>
      <br />
      <appactive :info="activeprojects"></appactive>
      <br /><br />
    </div>
    <hr class="container" />
    <div class="container">
      <h3>Contributors</h3>
      <contri :slides="slides"></contri>
    </div>
    <hr />
    <div class="container">
      <appfooter></appfooter>
    </div>
  </div>
</template>

<script>
import header from "./components/header";
import footer from "./components/footer";
import aim from "./components/aim";
import gridViewactive from "./components/gridViewactive";
import contributor from "./components/contributor";
import events from "./components/events";

export default {
  data: function () {
    return {
      completedprojects: [
        {
          title: "chatbot",
          body:
            "This chatbot helps the police in automating response from citizens",
          link: "https://github.com/Catalyst-CSE/Chat-Bot",
        },
      ],
      activeprojects: [
        {
          title: "IOS app",
          subtitle: "OpenSourceEvents-IOS",
          body:
            "This iOS-application contains a list of open source events and hackathons",
          link: "https://github.com/Catalyst-CSE/OpenSourceEvents-iOS",
          imageLink: "ios-app.png",
        },
        {
          title: "Website",
          subtitle: "OpenSourceEvents-Frontend",
          body:
            "This website contains a list of open source events and hackathons",
          link: "https://opensourcefrontend.netlify.app/",
          imageLink: "logo.png",
        },
      ],
    };
  },
  components: {
    appheader: header,
    appfooter: footer,
    appaim: aim,
    appactive: gridViewactive,
    contri: contributor,
    appevents: events,
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
