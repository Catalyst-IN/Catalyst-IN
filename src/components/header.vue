<template>
  <div class="row">
    <div class="col-lg-3 col-md-3 col-sm-6">
      <img
        @click="change3('home')"
        src="../assets/logo.png"
        class="img-thumbnail logo"
        width="200"
        height="200"
      />
    </div>
    <div class="col-lg-9 col-md-9 col-sm-6">
      <div id="iconText">
        <ul id="icons">
          <a href="https://github.com/Catalyst-IN" target="_blank">
            <li>
              <i class="fab fa-github"></i>
            </li>
          </a>
          <a href="https://twitter.com/Catalyst_IND" target="_blank">
            <li>
              <i class="fab fa-twitter"></i>
            </li>
          </a>
          <a
            href="https://www.linkedin.com/company/catalyst-smvd/"
            target="_blank"
          >
            <li>
              <i class="fab fa-linkedin"></i>
            </li>
          </a>
          <a href="https://discord.gg/EwpwF3s" target="_blank">
            <li>
              <i class="fab fa-discord"></i>
            </li>
          </a>
          <a href="mailto:catalystorg@hotmail.com" target="_blank">
            <li>
              <i class="fas fa-envelope"></i>
            </li>
          </a>
        </ul>
      </div>
      <hr id="divider" />
      <div class="header-nav">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
          <button
            class="navbar-toggler ml-auto"
            type="button"
            data-toggle="collapse"
            data-target="#navbarText"
            aria-controls="navbarText"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarText">
            <ul class="navbar-nav mr-auto">
              <li class="nav-item">
                <button
                  class="btn bt-nav"
                  type="button"
                  @click="change3('home')"
                >
                  Home
                </button>
              </li>
              <li class="nav-item">
                <button
                  class="btn bt-nav"
                  type="button"
                  @click="change1('whoweare')"
                >
                  Who we are
                </button>
              </li>
              <li class="nav-item">
                <button
                  class="btn bt-nav"
                  type="button"
                  @click="change2('whatwedo')"
                >
                  What we do
                </button>
              </li>
              <li class="nav-item">
                <a href="#events"
                  ><button
                    class="btn bt-nav"
                    type="button"
                    @click="change3('home')"
                  >
                    Events
                  </button></a
                >
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    change1(item) {
      this.$emit("namewasreset", item);
    },
    change2(item) {
      this.$emit("namewasreset", item);
    },
    change3(item) {
      this.$emit("namewasreset", item);
    },
  },
};
</script>

<style scoped>
img {
  cursor: pointer;
}
.logo {
  margin-top: 10px;
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

#icons li i {
  font-size: 35px;
  color: rgba(61, 55, 55, 0.808);
}

#icons a:nth-child(1) i:hover {
  color: #211f1f;
}

#icons a:nth-child(2) i:hover {
  color: #1da1f2;
}

#icons a:nth-child(3) i:hover {
  color: #0072b1;
}

#icons a:nth-child(4) i:hover {
  color: #738adb;
}

#icons a:nth-child(5) i:hover {
  color: black;
}

#icons {
  padding-left: 60%;
  padding-top: 5%;
}

.flexdisplay {
  display: flex;
}

#iconText {
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
  padding-left: 50px;
  padding-right: 50px;
  margin-left: 10px;
  margin-right: 10px;
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

.btn:focus {
  outline: none;
}

@media (max-width: 1200px) {
  #iconText {
    width: 550px;
  }

  #icons li i {
    font-size: 25px;
  }
  .bt-nav {
    padding-left: 40px;
    padding-right: 40px;
    margin-left: 5px;
    margin-right: 5px;
  }
}
</style>
