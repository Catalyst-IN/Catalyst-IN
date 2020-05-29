<template>
  <div class="flexdisplay">
    <div>
      <img
        @click="change4"
        src="../assets/logo.png"
        class="img-thumbnail logo"
        width="200"
        height="200"
      />
    </div>
    <div>
      <div id="navbarText">
        <ul id="icons">
          <a href="#">
            <li>
              <img
                src="../assets/iconfinder_github_rounded_394187.png"
                height="40px"
                width="40px"
              />
            </li>
          </a>
          <a href="#">
            <li>
              <img
                src="../assets/iconfinder_1_Twitter_colored_svg_5296514.png"
                height="40px"
                width="40px"
              />
            </li>
          </a>
          <a href="#">
            <li>
              <img
                src="../assets/iconfinder_1_Linkedin_unofficial_colored_svg_5296501.png"
                height="40px"
                width="40px"
              />
            </li>
          </a>
          <a href="#">
            <li>
              <img
                src="../assets/iconfinder_008_Mail_183573.png"
                height="40px"
                width="40px"
              />
            </li>
          </a>
          <a href="#">
            <li>
              <img
                src="../assets/iconfinder_1_Facebook_colored_svg_copy_5296499.png"
                height="40px"
                width="40px"
              />
            </li>
          </a>
        </ul>
      </div>
      <hr id="divider" />
      <div>
        <nav class="navbar navbar-light bg-light">
          <form class="form-inline">
            <button class="btn bt-nav" type="button" @click="change3">
              Home
            </button>
            <button class="btn bt-nav" type="button" @click="change1">
              Who we are
            </button>
            <button class="btn bt-nav" type="button" @click="change2">
              What we do
            </button>
            <a href="#events"><button class="btn bt-nav" type="button" @click="change3">
              Events
            </button></a>
          </form>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["selected"],
  methods: {
    change1() {
      this.selected = "whoweare";
      this.$emit("namewasreset", this.selected);
    },
    change2() {
      this.selected = "whatwedo";
      this.$emit("namewasreset", this.selected);
    },
    change3() {
      this.selected = "home";
      this.$emit("namewasreset", this.selected);
    }
  }
};
</script>

<style scoped>

img {
  cursor: pointer;
}
.logo {
  margin: 10px;
  z-index: 10;
}
.header {
  padding: 20px;
  position: relative;
  border-bottom: 2px solid yellow;
}
#icons li {
  display: inline;
  display: inline-block;
  list-style-type: none;
  padding-right: 20px;
}

ul {
  padding-left: 60%;
  padding-top: 5%;
}

.flexdisplay {
  display: flex;
}

#navbarText {
  float: right;
  width: 800px;
  height: 100px;
}

#divider {
  margin-top: 6rem;
  color: palevioletred;
  background-color: palevioletred;
}

.bt-nav {
  padding-left: 60px;
  padding-right: 60px;
  margin-left: 5px;
  margin-right: 5px;
  border: 1px solid #f8ba26;
  font-weight: bold;
}

.bt-nav:hover {
  background-color: #f8ba26;
  color: white;
}

.bt-nav:hover a {
  color: white;
  text-decoration: none;
}

.bt-nav a {
  color: black;
}

.btn:focus{
  outline:none;
}
</style>
