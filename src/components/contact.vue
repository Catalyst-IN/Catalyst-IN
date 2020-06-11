<template>
    <div class="container">
        <h3>
            Contact Us
        </h3>
        <p>
            Have a question? We can help. Please select the type of inquiry you
            have, and we’ll direct you to the correct place.
        </p>
        <div class="row">
            <!--Grid column-->
            <div class="col-md-9 mb-md-0 mb-5">
                <form id="contact-form" name="contact-form" method="POST">
                    <!--Grid row-->
                    <div class="row">
                        <!--Grid column-->
                        <div class="col-md-6">
                            <div class="md-form mb-0">
                                <input
                                    type="text"
                                    id="name"
                                    name="name"
                                    class="form-control"
                                    v-model="user.name"
                                    required
                                />
                                <label for="name" class="">Your name</label>
                            </div>
                        </div>
                        <!--Grid column-->

                        <!--Grid column-->
                        <div class="col-md-6">
                            <div class="md-form mb-0">
                                <input
                                    type="email"
                                    id="email"
                                    name="email"
                                    class="form-control"
                                    v-model="user.email"
                                    required
                                />
                                <label for="email" class="">Your email</label>
                            </div>
                        </div>
                        <!--Grid column-->
                    </div>
                    <!--Grid row-->

                    <!--Grid row-->
                    <div class="row">
                        <div class="col-md-12">
                            <div class="md-form mb-0">
                                <input
                                    type="text"
                                    id="subject"
                                    name="subject"
                                    class="form-control"
                                    v-model="user.subject"
                                    required
                                />
                                <label for="subject" class="">Subject</label>
                            </div>
                        </div>
                    </div>
                    <!--Grid row-->

                    <!--Grid row-->
                    <div class="row">
                        <!--Grid column-->
                        <div class="col-md-12">
                            <div class="md-form">
                                <textarea
                                    type="text"
                                    id="message"
                                    name="message"
                                    rows="2"
                                    class="form-control md-textarea"
                                    v-model="user.querymessage"
                                    required
                                ></textarea>
                                <label for="message">Your message</label>
                            </div>
                        </div>
                    </div>
                    <!--Grid row-->
                </form>
                <button class="btn btn-primary" @click.prevent="issubmit">
                    Send
                </button>
                <br /><br />
                <div class="alert alert-success" v-if="submitted">
                    Your response has been submitted.
                </div>
                <div class="alert alert-warning" v-if="notsubmitted">
                    Submit correct data.
                </div>
            </div>
            <!--Grid column-->

            <!--Grid column-->
            <div class="col-md-3 text-center">
                <ul class="list-unstyled mb-0">
                    <li>
                        <i class="fas fa-map-marker-alt fa-2x"></i>
                        <p>INDIA</p>
                    </li>

                    <li>
                        <i class="fas fa-phone mt-4 fa-2x"></i>
                        <p>+91 6005433494</p>
                    </li>

                    <li>
                        <i class="fas fa-envelope mt-4 fa-2x"></i>
                        <p>catalystorg@hotmail.com</p>
                    </li>
                </ul>
            </div>
            <!--Grid column-->
        </div>
    </div>
</template>

<script>
export default {
    name: 'contact',
    data: function () {
        return {
            submitted: false,
            notsubmitted: false,
            user: {
                name: null,
                email: null,
                subject: null,
                querymessage: null,
            },
        };
    },
    methods: {
        issubmit: function () {
            if (
                this.user.name !== null &&
                this.user.email !== null &&
                this.user.subject !== null &&
                this.user.querymessage !== null
            ) {
                this.submitted = true;
                this.notsubmitted = false;
                this.$http;
                this.user.name = null;
                this.user.email = null;
                this.user.subject = null;
                this.user.querymessage = null;
            } else {
                this.notsubmitted = true;
                this.submitted = false;
            }
        },
    },
};
</script>

<style scoped></style>
