<template>
  <div class="col-sm-6 col-md-4 col-lg-3">
    <div id="root">
      <div class="box">
        <div class="content">
          <slot name="title" class="title"></slot>
          <hr />
          <slot name="body" class="content"></slot>
          <br />
          <slot name="link"></slot>
          <p class="img__description" id="font">
            Contributors <br /><slot name="list"></slot>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,400;0,700;0,900;1,400&display=swap");

* {
  margin: 0;
  padding: 0;
  outline: 0;
  box-sizing: border-box;
}

html,
body,
#root {
  height: 100%;
}

#root {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
body {
  font-family: "Ubuntu", sans-serif;
}
#root .box {
  width: 270px;
  height: 350px;
  margin: 20px 20px 20px 20px;
  padding: 1rem;
  border-radius: 4px;
  background: #f8ba26;
  /* box-shadow: 0 3px 5px rgba(0, 0, 0, 0.18); */
  box-shadow: 5px 10px 8px #888888;
  color: white;
  display: flex;
  position: relative;
  flex-direction: colunm;
  transition: all 0.5s ease-in-out;
  border-image-slice: 1;
  overflow: hidden;
  transition: width 2s, height 2s;
}

#root .box .content p {
  font-size: 20px;
}

#root .box .content * {
  margin-bottom: 20px;
  line-height: 1;
}

.title {
  text-align: center;
}

#root .box:hover {
  width: 350px;
  height: 450px;
}

a,
a:hover {
  color: white;
  text-decoration: none;
}
.img__description {
  font-family: "Ubuntu", sans-serif;
  color: #fff;
  visibility: hidden;
  opacity: 0;
  font-size: 14px;
  /* transition effect. not necessary */
  transition: opacity 0.2s, visibility 0.2s;
}
.box:hover .img__description {
  visibility: visible;
  text-align: center;
  opacity: 1;
}
</style>
