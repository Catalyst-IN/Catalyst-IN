<template>
  <div class="container">
    <h3>
      Contact Us
    </h3>
    <p>
      Have a question? We can help. Please select the type of inquiry you have,
      and we’ll direct you to the correct place.
    </p>
    <div class="row">
      <!--Grid column-->
      <div class="col-md-9 mb-md-0 mb-5">
        <form
          id="contact-form"
          name="contact-form"
          action="mail.php"
          method="POST"
        >
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
                  v-model="name"
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
                  v-model="email"
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
                  v-model="subject"
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
                  v-model="querymessage"
                  required
                ></textarea>
                <label for="message">Your message</label>
              </div>
            </div>
          </div>
          <!--Grid row-->

          <input
            type="submit"
            @click.prevent="issubmit"
            value="Send"
            class="btn btn-primary"
          />
        </form>
        <div class="status" v-show="submitted">
          Your response has been submitted.
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
  name: "contact",
  data: function () {
    return {
      submitted: false,
      name: null,
      email: null,
      subject: null,
      querymessage: null,
    };
  },
  methods: {
    issubmit: function () {
      if (
        this.name !== null &&
        this.email !== null &&
        this.subject !== null &&
        this.querymessage !== null
      )
        this.submitted = true;
    },
  },
};
</script>

<style scoped>
.status {
  color: red;
}
</style>
