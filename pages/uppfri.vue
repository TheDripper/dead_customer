<template>
  <div id="root" class="w-full">
    <div id="intro" class="mx-auto">
      <img src="/pablo.jpg" id="imakid" />
      <h1 class="blink">U.P.P.F.R.I.</h1>
    </div>
    </div>
</template>
<style scoped lang="scss">
html,
body {
  background: #00ffff;
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}
p,
li {
  color: black;
  font-size: 24px;
  margin: 0 auto;
  font-family: "fira";
  line-height: 1.6;
}

p,
ul {
  max-width: 800px;
  width: 100%;
  margin: 0 auto;
  padding: 0.5rem;
  box-sizing: border-box;
}
h1 {
  font-family: "vcr";
  text-align: left;
  max-width: 600px;
  margin: 2rem auto;
  display: block;
  color: magenta;
  text-transform: uppercase;
  text-decoration: none;
  text-align: center;
  font-size: 40px;
  @media (min-width: 1000px) {
    font-size: 80px;
  }
}
a {
  text-decoration: none;
}

@font-face {
  font-family: "vcr";
  src: url("/vcr.ttf");
}
@font-face {
  font-family: "fira";
  src: url("/FiraCode-Regular.ttf");
}
video {
  width: 100vw;
  margin-bottom: 40px;
}
#more {
  color: white;
}
img {
  margin: 0 auto;
  display: block;
}
a {
  color: white;
}
.blink {
  animation: blink-animation 2s steps(5, start) infinite;
  -webkit-animation: blink-animation 2s steps(5, start) infinite;
}
@keyframes blink-animation {
  to {
    visibility: hidden;
  }
}
@-webkit-keyframes blink-animation {
  to {
    visibility: hidden;
  }
}
#intro {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
#intro h1 {
  color: white;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  white-space: nowrap;
  margin: 0;
  text-shadow: 5px 5px 0 black, -5px -5px 0 black, -5px 5px 0 black,
    5px -5px 0 black;
  font-size: 50px;
  @media (min-width: 1000px) {
    font-size: 80px;
  }
}
#imakid {
  width: 100vw;
}
#root {
  background: cyan;
}
.magenta {
  color: magenta;
}
a {
  color: blue;
  border-bottom: 2px solid magenta;
}
.speech {
  font-size: 30px !important;
  text-shadow: 2px 2px 0 black;
  color: magenta;
  font-weight: medium;
}
.frame {
  height: 0;
  width: 100%;
  padding-bottom: 56.25%;
  position: relative;
  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
}
</style>