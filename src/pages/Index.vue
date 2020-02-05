<template>
  <Layout>
  <div class="big-logo">
  <div class="big-logo-subtitle text-center">
  direction | design | development <br>  freelance digital creator <br> based in amsterdam, the netherlands
  </div>
  <video autoplay playsinline muted loop preload poster="https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/oceanshot.jpg">
  <source src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/ocean-small.webm" />
  <source src="http://thenewcode.com/assets/videos/ocean-small.mp4" />
</video>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 285 80" preserveAspectRatio="xMidYMin meet">
  <defs>
  <mask id="mask" x="0" y="0" width="100%" height="100%" >
    <rect x="0" y="0" width="100%" height="100%" style="fill:#FFF"/>
  <text x="50%"  y="50%" text-anchor="middle">JANNEMAN</text>
    </mask>
</defs>
<rect x="0" y="0" width="100%" height="100%" />
</svg>
</div>
<div class="introduction">
    <h1 class="mb-4">Hi There! Nice to meet you. <br> I am Janneman.</h1>
    <p>
    My real name is Jan Tijssen. I was born in 1983.
    </p>
    </div>


  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Gridsome starter bootstrap'
  }
}

const video = document.querySelector("video");
if (window.matchMedia('(prefers-reduced-motion)').matches) {
  video.removeAttribute("autoplay");
  video.pause();
}
</script>

<style>


@font-face {
  font-family: Biko;
  src:url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/biko-black.woff");
}
body {
  background: black;
  margin-top: 2rem;
}

.big-logo {
height: 100vh;

}

.introduction {
height: 100vh;

}

.big-logo-subtitle {
color: white;
font-family: anonymous-pro, monospace;
font-weight: 400;
font-style: normal;
font-size: 16px;
position: absolute;
    left: 50%;
    transform: translate(-50%, 0);
    top: 50%;
z-index: 100;
margin-left: auto;
margin-right: auto;
}

video {
width: 100%;
}

svg {
  width: 100%;
  position: absolute;
  left: 0;
  height: 100%;
  top: 130px;
  opacity: 0.9;
}
svg text {
  font-family: nimbus-sans-extended, sans-serif;
  font-weight: 900;
  text-transform: uppercase;
  font-size: 28px;
}


svg rect {
  fill: #000;
}
svg > rect {
    -webkit-mask: url(#mask);
    mask: url(#mask);
}
</style>
