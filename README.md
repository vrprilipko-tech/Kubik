[index.html](https://github.com/user-attachments/files/25621866/index.html)
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="2685.3">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 13.0px 'Helvetica Neue'; color: #000000}
    p.p2 {margin: 0.0px 0.0px 0.0px 0.0px; font: 13.0px 'Helvetica Neue'; color: #000000; min-height: 15.0px}
    span.s1 {color: #04359d}
  </style>
</head>
<body>
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html lang="ru"&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1">&lt;meta charset="UTF-8"&gt;</p>
<p class="p1">&lt;title&gt;Сакральный кубик&lt;/title&gt;</p>
<p class="p1">&lt;style&gt;</p>
<p class="p1">body {</p>
<p class="p1"><span class="Apple-converted-space">  </span>margin:0;</p>
<p class="p1"><span class="Apple-converted-space">  </span>height:100vh;</p>
<p class="p1"><span class="Apple-converted-space">  </span>display:flex;</p>
<p class="p1"><span class="Apple-converted-space">  </span>flex-direction:column;</p>
<p class="p1"><span class="Apple-converted-space">  </span>justify-content:center;</p>
<p class="p1"><span class="Apple-converted-space">  </span>align-items:center;</p>
<p class="p1"><span class="Apple-converted-space">  </span>font-family: serif;</p>
<p class="p1"><span class="Apple-converted-space">  </span>background:<span class="s1">#fff</span>;</p>
<p class="p1"><span class="Apple-converted-space">  </span>color:#000;</p>
<p class="p1"><span class="Apple-converted-space">  </span>perspective:1200px;</p>
<p class="p1">}</p>
<p class="p1">.scene {</p>
<p class="p1"><span class="Apple-converted-space">  </span>width:240px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>height:240px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>position:relative;</p>
<p class="p1"><span class="Apple-converted-space">  </span>margin-bottom:30px;</p>
<p class="p1">}</p>
<p class="p1">.tetrahedron {</p>
<p class="p1"><span class="Apple-converted-space">  </span>width:100%;</p>
<p class="p1"><span class="Apple-converted-space">  </span>height:100%;</p>
<p class="p1"><span class="Apple-converted-space">  </span>position:absolute;</p>
<p class="p1"><span class="Apple-converted-space">  </span>transform-style: preserve-3d;</p>
<p class="p1"><span class="Apple-converted-space">  </span>transition: transform 1.5s ease;</p>
<p class="p1">}</p>
<p class="p1">.face {</p>
<p class="p1"><span class="Apple-converted-space">  </span>position:absolute;</p>
<p class="p1"><span class="Apple-converted-space">  </span>width:240px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>height:240px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>display:flex;</p>
<p class="p1"><span class="Apple-converted-space">  </span>justify-content:center;</p>
<p class="p1"><span class="Apple-converted-space">  </span>align-items:center;</p>
<p class="p1"><span class="Apple-converted-space">  </span>font-size:60px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>font-weight:bold;</p>
<p class="p1"><span class="Apple-converted-space">  </span>clip-path: polygon(50% 0%, 0% 100%, 100% 100%);</p>
<p class="p1"><span class="Apple-converted-space">  </span>border:2px solid #000;</p>
<p class="p1"><span class="Apple-converted-space">  </span>background:<span class="s1">#eee</span>;</p>
<p class="p1">}</p>
<p class="p1">.face1 { transform: rotateY(0deg) translateZ(120px); }</p>
<p class="p1">.face2 { transform: rotateY(120deg) translateZ(120px); }</p>
<p class="p1">.face3 { transform: rotateY(240deg) translateZ(120px); }</p>
<p class="p1">.face4 { transform: rotateX(90deg) translateZ(120px); }</p>
<p class="p1">button {</p>
<p class="p1"><span class="Apple-converted-space">  </span>padding:12px 30px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>font-size:16px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>border-radius:8px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>border:1px solid #000;</p>
<p class="p1"><span class="Apple-converted-space">  </span>cursor:pointer;</p>
<p class="p1"><span class="Apple-converted-space">  </span>background:<span class="s1">#ddd</span>;</p>
<p class="p1">}</p>
<p class="p1">button:hover { background:<span class="s1">#ccc</span>; }</p>
<p class="p1">&lt;/style&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p1">&lt;body&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;div class="scene"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div class="tetrahedron" id="tetra"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="face face1"&gt;−&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="face face2"&gt;+&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="face face3"&gt;+⁄−&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="face face4"&gt;•&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/div&gt;</p>
<p class="p1">&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;button onclick="roll()"&gt;Бросить кубик&lt;/button&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;script&gt;</p>
<p class="p1">const tetra = document.getElementById("tetra");</p>
<p class="p1">const rotations = [</p>
<p class="p1"><span class="Apple-converted-space">  </span>{x:0,y:0},</p>
<p class="p1"><span class="Apple-converted-space">  </span>{x:0,y:-120},</p>
<p class="p1"><span class="Apple-converted-space">  </span>{x:0,y:-240},</p>
<p class="p1"><span class="Apple-converted-space">  </span>{x:-90,y:0}</p>
<p class="p1">];</p>
<p class="p1">function roll(){</p>
<p class="p1"><span class="Apple-converted-space">  </span>const random = Math.floor(Math.random()*rotations.length);</p>
<p class="p1"><span class="Apple-converted-space">  </span>const extra = 720;</p>
<p class="p1"><span class="Apple-converted-space">  </span>tetra.style.transform=`rotateX(${rotations[random].x+extra}deg) rotateY(${rotations[random].y+extra}deg)`;</p>
<p class="p1">}</p>
<p class="p1">&lt;/script&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
