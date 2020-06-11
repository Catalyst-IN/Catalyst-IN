<template>
    <div>
        <div class="container">
            <appaim></appaim>
            <hr />
        </div>
        <div class="container" id="events">
            <h3>Events</h3>
            <br />
            <appevents></appevents>
        </div>
        <hr class="container" />
        <div class="container">
            <h3>Active projects</h3>
            <br />
            <appactive :info="activeprojects"></appactive>
            <br />
            <br />
            <button class="btn btn-info" style="float: right;">
                <a href="https://github.com/Catalyst-IN">See More..</a>
            </button>
            <br /><br />
        </div>
        <div class="container">
            <hr />
            <h3>Core Team</h3>
            <contri :slides="slides"></contri>
        </div>
        <br />
        <div class="container">
            <hr />
            <h3>How Can I Support CATALYST</h3>
            <br />
            <appsupport></appsupport>
            <br />
        </div>
    </div>
</template>

<script>
import aim from './components/aim';
import gridViewactive from './components/gridViewactive';
import contributor from './components/contributor';
import events from './components/events';
import support from './components/support';

export default {
    data: function () {
        return {
            completedprojects: [
                {
                    title: 'chatbot',
                    body:
                        'This chatbot helps the police in automating response from citizens',
                    link: 'https://github.com/Catalyst-CSE/Chat-Bot',
                },
            ],
            activeprojects: [
                {
                    title: 'IOS app',
                    subtitle: 'OpenSourceEvents-IOS',
                    body:
                        'This iOS-application contains a list of open source events and hackathons',
                    link:
                        'https://github.com/Catalyst-CSE/OpenSourceEvents-iOS',
                    imageLink: 'ios-app.png',
                },
                {
                    title: 'Website',
                    subtitle: 'OpenSourceEvents-Frontend',
                    body:
                        'This website contains a list of open source events and hackathons',
                    link: 'https://opensourcefrontend.netlify.app/',
                    imageLink: 'logo.png',
                },
                {
                    title: 'Collection of events',
                    subtitle: 'Open-Source-Events',
                    body:
                        'This is a collection of Open Source events and Hackathons. Students always forget the dates of Open Source event and recall after the date is over to fill the form.',
                    link: 'https://github.com/Catalyst-IN/Open-Source-Events',
                    imageLink: 'open.png',
                },
            ],
        };
    },
    components: {
        appaim: aim,
        appactive: gridViewactive,
        contri: contributor,
        appevents: events,
        appsupport: support,
    },
};
</script>

<style scoped>
button a {
    color: white;
}

button a:hover {
    text-decoration: none;
}
h3 {
    color: black;
    font-family: 'Ubuntu', sans-serif;
}
</style>
