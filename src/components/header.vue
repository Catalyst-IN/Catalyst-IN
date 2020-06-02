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
        <nav class="navbar navbar-light bg-light">
          <form class="form-inline">
            <button class="btn bt-nav" type="button" @click="change3('home')">
              Home
            </button>
            <button
              class="btn bt-nav"
              type="button"
              @click="change1('whoweare')"
            >
              Who we are
            </button>
            <button
              class="btn bt-nav"
              type="button"
              @click="change2('whatwedo')"
            >
              What we do
            </button>
            <a href="#events"
              ><button
                class="btn bt-nav"
                type="button"
                @click="change3('home')"
              >
                Events
              </button></a
            >
          </form>
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

#icons li i {
  font-size: 35px;
  color: rgba(61, 55, 55, 0.808);
}

#icons a:nth-child(1) i:hover {
  font-size: 35px;
  color: #211f1f;
}

#icons a:nth-child(2) i:hover {
  font-size: 35px;
  color: #1da1f2;
}

#icons a:nth-child(3) i:hover {
  font-size: 35px;
  color: #0072b1;
}

#icons a:nth-child(4) i:hover {
  font-size: 35px;
  color: #738adb;
}

#icons a:nth-child(5) i:hover {
  font-size: 35px;
  color: black;
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

.btn:focus {
  outline: none;
}

@media (max-width: 1200px) {
  #navbarText {
    width: 550px;
  }

  #icons li i {
    font-size: 25px;
  }

  .bt-nav {
    padding-left: 30px;
    padding-right: 30px;
    margin-left: 5px;
    margin-right: 5px;
  }
}

@media (max-width: 1000px) {
  .bt-nav {
    padding-left: 15px;
    padding-right: 15px;
    margin-left: 5px;
    margin-right: 5px;
  }
}

@media (max-width: 600px) {
  #navbarText {
    width: 200px;
  }
  #icons li i {
    font-size: 15px;
  }
  .header-nav {
    width: 300px;
  }

  .bt-nav {
    padding-left: 15px;
    padding-right: 15px;
    margin-left: 10px;
    margin-right: 10px;
  }

  #divider {
    width: 100px;
  }
}
</style>
