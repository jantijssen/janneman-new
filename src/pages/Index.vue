<template>
  <Layout>
  <div class="big-logo">
  <div class="big-logo-subtitle text-center">
  direction | design | development <br>  freelance digital creator <br> based in amsterdam, the netherlands
  </div>
  <video autoplay playsinline muted loop class="big-video">
  <source src="../assets/video/home-bg.webm" />
  <source src="../assets/video/home-bg.mp4" />
</video>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 285 80" preserveAspectRatio="xMidYMin slice">
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
position: absolute;
 right: 0;
 bottom: 0;
 min-width: 100%;
 min-height: 100%;
 z-index: 0;
}

svg {
  width: 100%;
  position: absolute;
  left: 0;
  height: 100%;
  top: 0;
  opacity: 0.88;
}
svg text {
  font-family: nimbus-sans-extended, sans-serif;
  font-weight: 900;
  text-transform: uppercase;
  font-size: 14px;
}

.big-video {
height: 100vh;
}


svg rect {
  fill: #000;
}
svg > rect {
    -webkit-mask: url(#mask);
    mask: url(#mask);
}
</style>
