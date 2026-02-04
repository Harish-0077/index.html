# index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>DevOps Using MANET Concepts – Slideshow</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Segoe UI, Arial, sans-serif;
}

body{
    background:#0f172a;
    overflow:hidden;
}

/* radio */
input{ display:none; }

.slides{
    position:relative;
    width:100vw;
    height:100vh;
}

/* slide */
.slide{
    position:absolute;
    width:100%;
    height:100%;
    padding:60px 80px;
    background:#f8fafc;
    opacity:0;
    transform:translateX(100%);
    transition:.6s;
    display:flex;
    flex-direction:column;
    justify-content:center;
}

/* show */
#s1:checked ~ .slides .slide:nth-child(1),
#s2:checked ~ .slides .slide:nth-child(2),
#s3:checked ~ .slides .slide:nth-child(3),
#s4:checked ~ .slides .slide:nth-child(4),
#s5:checked ~ .slides .slide:nth-child(5),
#s6:checked ~ .slides .slide:nth-child(6),
#s7:checked ~ .slides .slide:nth-child(7),
#s8:checked ~ .slides .slide:nth-child(8),
#s9:checked ~ .slides .slide:nth-child(9){
    opacity:1;
    transform:translateX(0);
}

/* typography */
h1{font-size:42px;margin-bottom:20px;}
h2{font-size:32px;margin-bottom:20px;color:#2563eb;}
p{margin-bottom:12px;font-size:18px;}
ul{margin-left:20px;font-size:18px;}

/* layout */
.row{
    display:flex;
    gap:40px;
}

.card{
    flex:1;
    background:white;
    padding:20px;
    border-radius:10px;
    box-shadow:0 6px 14px rgba(0,0,0,.08);
}

/* images */
.slide img{
    max-width:70%;
    height:260px;
    object-fit:contain;
    margin:25px auto 0;
    border-radius:10px;
}

/* pipeline */
.pipeline{
    display:flex;
    gap:15px;
    margin-top:20px;
}
.box{
    background:#2563eb;
    color:white;
    padding:14px 20px;
    border-radius:6px;
}

/* nav */
.nav{
    position:absolute;
    bottom:25px;
    right:40px;
}
.nav label{
    background:#2563eb;
    color:white;
    padding:10px 18px;
    margin-left:8px;
    border-radius:6px;
    cursor:pointer;
}
</style>
</head>

<body>

<!-- radios -->
<input type="radio" name="slide" id="s1" checked>
<input type="radio" name="slide" id="s2">
<input type="radio" name="slide" id="s3">
<input type="radio" name="slide" id="s4">
<input type="radio" name="slide" id="s5">
<input type="radio" name="slide" id="s6">
<input type="radio" name="slide" id="s7">
<input type="radio" name="slide" id="s8">
<input type="radio" name="slide" id="s9">

<div class="slides">

<!-- Slide 1 -->
<div class="slide">
<h1>DevOps Explained Using MANET Concepts</h1>
<p>Understanding modern DevOps practices through Mobile Ad-hoc Network principles.</p>
<img src="images/img1.jpg.jpg">
<div class="nav"><label for="s2">Next →</label></div>
</div>

<!-- Slide 2 -->
<div class="slide">
<h2>Why Compare MANET with DevOps?</h2>
<ul>
<li>No central control</li>
<li>High adaptability</li>
<li>Continuous change</li>
<li>Automation for stability</li>
</ul>
<img src="images/img2.png">
<div class="nav"><label for="s1">← Prev</label><label for="s3">Next →</label></div>
</div>

<!-- Slide 3 -->
<div class="slide">
<h2>Infrastructure-less → Cloud Infrastructure</h2>
<div class="row">
<div class="card">
<b>MANET</b>
<ul>
<li>No fixed routers</li>
<li>Self-configuring nodes</li>
<li>Temporary topology</li>
</ul>
</div>
<div class="card">
<b>DevOps</b>
<ul>
<li>Virtual servers</li>
<li>Containers</li>
<li>On-demand provisioning</li>
</ul>
</div>
</div>
<img src="images/img3.png">
<div class="nav"><label for="s2">← Prev</label><label for="s4">Next →</label></div>
</div>

<!-- Slide 4 -->
<div class="slide">
<h2>Dynamic Topology → Auto Scaling</h2>
<ul>
<li>Horizontal scaling</li>
<li>Load balancers</li>
<li>High availability</li>
</ul>
<img src="images/img4.png">
<div class="nav"><label for="s3">← Prev</label><label for="s5">Next →</label></div>
</div>

<!-- Slide 5 -->
<div class="slide">
<h2>Multi-hop Routing → CI/CD Pipeline</h2>
<div class="pipeline">
<div class="box">Code</div>
<div class="box">Build</div>
<div class="box">Test</div>
<div class="box">Deploy</div>
</div>
<img src="images/img5.png">
<div class="nav"><label for="s4">← Prev</label><label for="s6">Next →</label></div>
</div>

<!-- Slide 6 -->
<div class="slide">
<h2>MAC Protocols → Resource Management</h2>
<ul>
<li>CPU scheduling</li>
<li>Memory optimization</li>
<li>Kubernetes orchestration</li>
</ul>
<img src="images/img6.png">
<div class="nav"><label for="s5">← Prev</label><label for="s7">Next →</label></div>
</div>

<!-- Slide 7 -->
<div class="slide">
<h2>Routing Protocols → Deployment Strategies</h2>
<ul>
<li>Blue-Green</li>
<li>Canary</li>
<li>Rolling Updates</li>
</ul>
<img src="images/img7.png">
<div class="nav"><label for="s6">← Prev</label><label for="s8">Next →</label></div>
</div>

<!-- Slide 8 -->
<div class="slide">
<h2>Security in DevOps</h2>
<ul>
<li>Static scanning</li>
<li>Dependency checks</li>
<li>Image scanning</li>
<li>Monitoring</li>
</ul>
<img src="images/img8.png">
<div class="nav"><label for="s7">← Prev</label><label for="s9">Next →</label></div>
</div>

<!-- Slide 9 -->
<div class="slide">
<h2>Cross-Layer DevOps Integration</h2>
<ul>
<li>Dev + QA + Ops + Security</li>
<li>Shared responsibility</li>
<li>Faster delivery</li>
</ul>
<img src="images/img9.webp">
<div class="nav"><label for="s8">← Prev</label></div>
</div>

</div>

</body>
</html>
