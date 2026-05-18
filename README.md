


<img align='right' src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="230">



# <p><em>Telegram id <a href="http://www.telegram.com/@am_dq_fan">@am_dQ_fan</a><img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="50"> 


<a href="https://t.me/am_dq_fan"><img src="https://img.shields.io/badge/Join-Telegram%20Channel-red.svg?logo=Telegram"></a> <a href="https://t.me/am_dq_fan"><img src="https://img.shields.io/badge/Join-Telegram%20Group-blue.svg?logo=telegram"></a>




</em></p>

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FfireganqQ&count_bg=%231EE510&title_bg=%23555555&icon=&icon_color=%23931414&title=account+views&edge_flat=false)](https://github.com/dqanshi)

[![ dqanshi github stats](https://github-readme-stats.vercel.app/api?username=dqanshi&show_icons=true&theme=cobalt&count_private=true)](https://github.com/dqanshi)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=dqanshi&layout=compact&theme=cobalt)](https://github.com/dqanshi)

## <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> thug life...  













## 🎵 Now Playing

![Spotify Now Playing](https://novatorem.vercel.app/api/spotify?timestamp=123456)



<h3 alilefgn="left">i know :</h3>

<p align="left"> <a href="https://www.gnu.org/software/bash/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/> </a> <a href="https://www.blender.org/" target="_blank"> <img src="https://download.blender.org/branding/community/blender_community_badge_white.svg" alt="blender" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://cloud.google.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://grafana.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/grafana/grafana-icon.svg" alt="grafana" width="40" height="40"/> </a> <a href="https://heroku.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg" alt="heroku" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.adobe.com/in/products/illustrator.html" target="_blank"> <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://unrealengine.com/" target="_blank"> <img src="https://raw.githubusercontent.com/kenangundogan/fontisto/036b7eca71aab1bef8e6a0518f7329f13ed62f6b/icons/svg/brand/unreal-engine.svg" alt="unreal" width="40" height="40"/> </a> </p









<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>SPACE TIME LIVE</title>

<style>

body{
    margin:0;
    overflow:hidden;
    background:black;
}

canvas{
    display:block;
}

#time{
    position:absolute;
    top:20px;
    left:20px;
    color:#00ffff;
    font-size:28px;
    font-family:monospace;
    text-shadow:0 0 20px cyan;
    z-index:100;
}

#label{
    position:absolute;
    top:60px;
    left:20px;
    color:white;
    font-size:14px;
    font-family:Arial;
    z-index:100;
    letter-spacing:3px;
}

</style>
</head>

<body>

<div id="time"></div>
<div id="label">SPACE • TIME • LIVE</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>

<script>

//
// SCENE
//

const scene = new THREE.Scene();

const camera = new THREE.PerspectiveCamera(
75,
window.innerWidth/window.innerHeight,
0.1,
5000
);

const renderer = new THREE.WebGLRenderer({
antialias:true
});

renderer.setSize(
window.innerWidth,
window.innerHeight
);

document.body.appendChild(renderer.domElement);

camera.position.z = 30;

//
// STARS
//

const starsGeometry =
new THREE.BufferGeometry();

const starCount = 25000;

const positions =
new Float32Array(starCount * 3);

for(let i=0;i<starCount*3;i++){

    positions[i] =
    (Math.random()-0.5)*3000;

}

starsGeometry.setAttribute(
'position',
new THREE.BufferAttribute(
positions,
3
)
);

const starsMaterial =
new THREE.PointsMaterial({
color:0xffffff,
size:0.7
});

const stars =
new THREE.Points(
starsGeometry,
starsMaterial
);

scene.add(stars);

//
// EARTH
//

const loader =
new THREE.TextureLoader();

const earthTexture =
loader.load(
'https://threejs.org/examples/textures/planets/earth_atmos_2048.jpg'
);

const earthGeometry =
new THREE.SphereGeometry(
6,
128,
128
);

const earthMaterial =
new THREE.MeshStandardMaterial({
map:earthTexture
});

const earth =
new THREE.Mesh(
earthGeometry,
earthMaterial
);

scene.add(earth);

//
// SUN LIGHT
//

const sun =
new THREE.PointLight(
0xffffff,
2
);

sun.position.set(
50,
0,
50
);

scene.add(sun);

//
// AMBIENT LIGHT
//

const ambient =
new THREE.AmbientLight(
0x404040,
1.5
);

scene.add(ambient);

//
// GALAXY PARTICLES
//

const galaxyGeometry =
new THREE.BufferGeometry();

const galaxyCount = 12000;

const galaxyPos =
new Float32Array(galaxyCount * 3);

for(let i=0;i<galaxyCount;i++){

    const i3 = i * 3;

    const radius =
    Math.random() * 500;

    const angle =
    radius * 0.05;

    galaxyPos[i3] =
    Math.cos(angle) * radius;

    galaxyPos[i3+1] =
    (Math.random()-0.5)*50;

    galaxyPos[i3+2] =
    Math.sin(angle) * radius;
}

galaxyGeometry.setAttribute(
'position',
new THREE.BufferAttribute(
galaxyPos,
3
)
);

const galaxyMaterial =
new THREE.PointsMaterial({
color:0x00ffff,
size:0.5
});

const galaxy =
new THREE.Points(
galaxyGeometry,
galaxyMaterial
);

scene.add(galaxy);

//
// CLOCK
//

function updateClock(){

    const now =
    new Date();

    document.getElementById(
    "time"
    ).innerHTML =
    now.toUTCString();

}

setInterval(
updateClock,
1000
);

updateClock();

//
// ANIMATION
//

function animate(){

    requestAnimationFrame(
    animate
    );

    earth.rotation.y += 0.0015;

    stars.rotation.y += 0.00008;

    galaxy.rotation.y += 0.0003;

    renderer.render(
    scene,
    camera
    );
}

animate();

//
// RESIZE
//

window.addEventListener(
'resize',
()=>{

camera.aspect =
window.innerWidth /
window.innerHeight;

camera.updateProjectionMatrix();

renderer.setSize(
window.innerWidth,
window.innerHeight
);

});

</script>

</body>
</html>








