<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SEHUDIN | Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#050816;
    color:white;
    overflow-x:hidden;
}

/* BACKGROUND */

.bg{
    position:fixed;
    width:100%;
    height:100%;
    z-index:-1;
    overflow:hidden;
}

.bg span{
    position:absolute;
    display:block;
    width:220px;
    height:220px;
    background:rgba(14,165,233,0.08);
    border-radius:50%;
    animation:float 15s linear infinite;
}

.bg span:nth-child(1){
    top:10%;
    left:-5%;
}

.bg span:nth-child(2){
    bottom:5%;
    right:-5%;
}

.bg span:nth-child(3){
    top:50%;
    left:70%;
    width:120px;
    height:120px;
}

@keyframes float{
    0%{
        transform:translateY(0px) rotate(0deg);
    }

    50%{
        transform:translateY(-40px) rotate(180deg);
    }

    100%{
        transform:translateY(0px) rotate(360deg);
    }
}

/* NAVBAR */

nav{
    width:100%;
    padding:20px 8%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:fixed;
    top:0;
    z-index:1000;
    backdrop-filter:blur(10px);
    background:rgba(5,8,22,0.6);
}

.logo{
    font-size:24px;
    font-weight:700;
    color:#0EA5E9;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-size:14px;
    transition:0.3s;
}

nav ul li a:hover{
    color:#0EA5E9;
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:120px 8%;
    gap:50px;
    flex-wrap:wrap;
}

.hero-text{
    flex:1;
    min-width:300px;
}

.tag{
    display:inline-block;
    padding:10px 18px;
    background:rgba(14,165,233,0.1);
    border:1px solid rgba(14,165,233,0.3);
    border-radius:999px;
    color:#0EA5E9;
    margin-bottom:25px;
    font-size:14px;
}

.hero-text h1{
    font-size:70px;
    line-height:1.1;
    margin-bottom:20px;
}

.hero-text h1 span{
    color:#0EA5E9;
}

.hero-text p{
    color:#94A3B8;
    line-height:1.9;
    max-width:600px;
    margin-bottom:35px;
}

.buttons{
    display:flex;
    gap:20px;
    flex-wrap:wrap;
}

.btn{
    padding:15px 28px;
    border-radius:14px;
    text-decoration:none;
    font-weight:600;
    transition:0.3s;
}

.btn-primary{
    background:#0EA5E9;
    color:white;
}

.btn-primary:hover{
    transform:translateY(-5px);
    box-shadow:0 0 25px rgba(14,165,233,0.5);
}

.btn-secondary{
    border:1px solid rgba(255,255,255,0.1);
    color:white;
}

.btn-secondary:hover{
    background:rgba(255,255,255,0.05);
}

/* HERO CARD */

.hero-card{
    flex:1;
    min-width:300px;
    display:flex;
    justify-content:center;
}

.card{
    width:100%;
    max-width:400px;
    background:rgba(255,255,255,0.05);
    border:1px solid rgba(255,255,255,0.08);
    border-radius:30px;
    padding:30px;
    backdrop-filter:blur(20px);
    box-shadow:0 0 40px rgba(14,165,233,0.15);
}

.card img{
    width:100%;
    border-radius:20px;
    margin-bottom:20px;
}

.card h3{
    margin-bottom:10px;
}

.card p{
    color:#94A3B8;
    line-height:1.8;
}

/* SECTION */

section{
    padding:100px 8%;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-size:42px;
    margin-bottom:15px;
}

.section-title p{
    color:#94A3B8;
}

/* GRID */

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.box{
    background:rgba(255,255,255,0.04);
    border:1px solid rgba(255,255,255,0.06);
    padding:30px;
    border-radius:24px;
    transition:0.3s;
}

.box:hover{
    transform:translateY(-10px);
    box-shadow:0 0 30px rgba(14,165,233,0.15);
}

.box h3{
    margin-bottom:15px;
}

.box p{
    color:#94A3B8;
    line-height:1.8;
}

/* TECH */

.skills{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:15px;
}

.skill{
    padding:14px 22px;
    background:rgba(14,165,233,0.1);
    border:1px solid rgba(14,165,233,0.2);
    border-radius:999px;
    transition:0.3s;
}

.skill:hover{
    transform:translateY(-5px);
    background:#0EA5E9;
}

/* FOOTER */

footer{
    padding:40px 8%;
    text-align:center;
    border-top:1px solid rgba(255,255,255,0.06);
    color:#64748B;
}

/* MOBILE */

@media(max-width:900px){

    .hero{
        padding-top:150px;
    }

    .hero-text h1{
        font-size:50px;
    }

    nav ul{
        display:none;
    }

}

</style>
</head>
<body>

<!-- BACKGROUND -->
<div class="bg">
    <span></span>
    <span></span>
    <span></span>
</div>

<!-- NAVBAR -->
<nav>

    <div class="logo">SEHUDIN</div>

    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Experience</a></li>
        <li><a href="#">Skills</a></li>
        <li><a href="#">Contact</a></li>
    </ul>

</nav>

<!-- HERO -->
<section class="hero">

    <div class="hero-text">

        <div class="tag">
            ⚡ Software Engineer & Network Engineer
        </div>

        <h1>
            Building <span>Modern Networks</span> & Digital Solutions
        </h1>

        <p>
            Passionate in ISP Infrastructure, MikroTik Automation,
            Linux Server, Web Development, and creating reliable
            technology systems with modern innovation.
        </p>

        <div class="buttons">

            <a href="#" class="btn btn-primary">
                Explore Portfolio
            </a>

            <a href="#" class="btn btn-secondary">
                Contact Me
            </a>

        </div>

    </div>

    <div class="hero-card">

        <div class="card">

            <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=1200&auto=format&fit=crop">

            <h3>MikroTik • Linux • ISP</h3>

            <p>
                Reliable networking infrastructure and automation systems
                designed for modern internet services and enterprise solutions.
            </p>

        </div>

    </div>

</section>

<!-- EXPERIENCE -->
<section>

    <div class="section-title">
        <h2>Experience</h2>
        <p>Professional journey & infrastructure projects</p>
    </div>

    <div class="grid">

        <div class="box">
            <h3>PT. Powertel Indonesia</h3>

            <p>
                Fiber Optic Installation, MikroTik Administration,
                Network Monitoring, LAN & WiFi Deployment,
                CCTV Installation & Troubleshooting.
            </p>
        </div>

        <div class="box">
            <h3>Global Media Data Prima</h3>

            <p>
                Internet Installation, Wireless Configuration,
                Huawei & Ubiquiti Setup,
                Village Internet Infrastructure.
            </p>
        </div>

    </div>

</section>

<!-- SKILLS -->
<section>

    <div class="section-title">
        <h2>Tech Stack</h2>
        <p>Technology & tools I work with</p>
    </div>

    <div class="skills">

        <div class="skill">PHP</div>
        <div class="skill">Python</div>
        <div class="skill">React</div>
        <div class="skill">MySQL</div>
        <div class="skill">Linux</div>
        <div class="skill">MikroTik</div>
        <div class="skill">Cisco</div>
        <div class="skill">Huawei</div>
        <div class="skill">Ubiquiti</div>

    </div>

</section>

<!-- FOOTER -->
<footer>

    ⚡ Building Networks • Creating Solutions • Empowering Technology

</footer>

</body>
</html>
