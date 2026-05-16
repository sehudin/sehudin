<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>SEHUDIN - Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Poppins',sans-serif;
    background:#050816;
    color:white;
    overflow-x:hidden;
}

/* Background Animation */

.bg-animation{
    position:fixed;
    width:100%;
    height:100%;
    z-index:-1;
    overflow:hidden;
}

.circle{
    position:absolute;
    border-radius:50%;
    background:rgba(14,165,233,0.12);
    animation:float 10s infinite linear;
}

.circle:nth-child(1){
    width:250px;
    height:250px;
    top:10%;
    left:-5%;
}

.circle:nth-child(2){
    width:180px;
    height:180px;
    bottom:10%;
    right:-5%;
}

.circle:nth-child(3){
    width:120px;
    height:120px;
    top:50%;
    left:70%;
}

@keyframes float{
    0%{
        transform:translateY(0px) rotate(0deg);
    }
    50%{
        transform:translateY(-30px) rotate(180deg);
    }
    100%{
        transform:translateY(0px) rotate(360deg);
    }
}

/* Container */

.container{
    width:100%;
    max-width:450px;
    margin:auto;
    padding:20px;
}

/* Mobile Card */

.phone-ui{
    background:rgba(255,255,255,0.05);
    border:1px solid rgba(255,255,255,0.08);
    border-radius:35px;
    backdrop-filter:blur(20px);
    overflow:hidden;
    box-shadow:
    0 0 30px rgba(14,165,233,0.15),
    inset 0 0 20px rgba(255,255,255,0.03);
}

/* Header */

.hero{
    padding:40px 25px;
    text-align:center;
    background:
    linear-gradient(
        180deg,
        rgba(14,165,233,0.18),
        transparent
    );
}

.avatar{
    width:110px;
    height:110px;
    border-radius:50%;
    border:4px solid rgba(255,255,255,0.15);
    object-fit:cover;
    margin-bottom:18px;
    box-shadow:0 0 25px rgba(14,165,233,0.45);
}

.hero h1{
    font-size:32px;
    font-weight:700;
    letter-spacing:2px;
}

.hero p{
    margin-top:10px;
    color:#94A3B8;
    font-size:14px;
    line-height:1.7;
}

/* Typing */

.typing{
    color:#0EA5E9;
    font-weight:600;
    margin-top:18px;
    height:24px;
    overflow:hidden;
    position:relative;
}

.typing span{
    position:absolute;
    width:100%;
    opacity:0;
    animation:typing 12s infinite;
}

.typing span:nth-child(2){
    animation-delay:3s;
}

.typing span:nth-child(3){
    animation-delay:6s;
}

.typing span:nth-child(4){
    animation-delay:9s;
}

@keyframes typing{
    0%{
        opacity:0;
        transform:translateY(20px);
    }
    10%{
        opacity:1;
        transform:translateY(0);
    }
    25%{
        opacity:1;
    }
    35%{
        opacity:0;
        transform:translateY(-20px);
    }
    100%{
        opacity:0;
    }
}

/* Stats */

.stats{
    display:flex;
    justify-content:space-between;
    padding:0 20px 25px;
}

.stat-card{
    width:32%;
    background:rgba(255,255,255,0.04);
    border-radius:18px;
    padding:18px 10px;
    text-align:center;
    border:1px solid rgba(255,255,255,0.05);
}

.stat-card h2{
    color:#0EA5E9;
    font-size:20px;
}

.stat-card span{
    color:#94A3B8;
    font-size:12px;
}

/* Section */

.section{
    padding:20px;
}

.section-title{
    font-size:18px;
    margin-bottom:18px;
    font-weight:600;
    color:#0EA5E9;
}

/* Cards */

.card{
    background:rgba(255,255,255,0.04);
    border-radius:22px;
    padding:18px;
    margin-bottom:15px;
    border:1px solid rgba(255,255,255,0.05);
    transition:0.3s;
}

.card:hover{
    transform:translateY(-5px);
    box-shadow:0 0 20px rgba(14,165,233,0.15);
}

.card h3{
    margin-bottom:8px;
    font-size:17px;
}

.card p{
    color:#94A3B8;
    font-size:13px;
    line-height:1.8;
}

/* Skills */

.skills{
    display:flex;
    flex-wrap:wrap;
    gap:12px;
}

.skill{
    padding:10px 16px;
    background:rgba(14,165,233,0.1);
    border:1px solid rgba(14,165,233,0.2);
    border-radius:999px;
    font-size:13px;
}

/* Social */

.socials{
    display:flex;
    justify-content:center;
    gap:15px;
    margin-top:20px;
}

.socials a{
    width:50px;
    height:50px;
    border-radius:18px;
    background:rgba(255,255,255,0.05);
    display:flex;
    align-items:center;
    justify-content:center;
    text-decoration:none;
    color:white;
    font-size:22px;
    transition:0.3s;
}

.socials a:hover{
    background:#0EA5E9;
    transform:translateY(-5px);
}

/* Footer */

.footer{
    text-align:center;
    padding:25px;
    color:#64748B;
    font-size:13px;
}

/* Responsive */

@media(max-width:500px){

    .container{
        padding:10px;
    }

    .hero h1{
        font-size:28px;
    }

}

</style>
</head>
<body>

<div class="bg-animation">
    <div class="circle"></div>
    <div class="circle"></div>
    <div class="circle"></div>
</div>

<div class="container">

<div class="phone-ui">

    <!-- HERO -->
    <div class="hero">

        <img class="avatar" src="https://i.ibb.co/5M0K5xQ/profile.png">

        <h1>SEHUDIN</h1>

        <p>
            Software Engineer • Network Engineer • ISP Infrastructure
        </p>

        <div class="typing">
            <span>MikroTik Specialist</span>
            <span>Automation Enthusiast</span>
            <span>Linux Server Engineer</span>
            <span>Web Developer</span>
        </div>

    </div>

    <!-- STATS -->
    <div class="stats">

        <div class="stat-card">
            <h2>5+</h2>
            <span>Experience</span>
        </div>

        <div class="stat-card">
            <h2>50+</h2>
            <span>Projects</span>
        </div>

        <div class="stat-card">
            <h2>24/7</h2>
            <span>Support</span>
        </div>

    </div>

    <!-- ABOUT -->
    <div class="section">

        <div class="section-title">
            About Me
        </div>

        <div class="card">
            <p>
                Passionate Software Engineer and Network Engineer focused on
                building reliable infrastructure, ISP systems, automation,
                Linux servers, and modern networking solutions.
            </p>
        </div>

    </div>

    <!-- SKILLS -->
    <div class="section">

        <div class="section-title">
            Tech Stack
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

    </div>

    <!-- EXPERIENCE -->
    <div class="section">

        <div class="section-title">
            Experience
        </div>

        <div class="card">
            <h3>PT. Powertel Indonesia</h3>
            <p>
                Fiber Optic Installation, Network Monitoring,
                MikroTik Administration, CCTV Installation,
                LAN & WiFi Deployment.
            </p>
        </div>

        <div class="card">
            <h3>Global Media Data Prima</h3>
            <p>
                Wireless Configuration, Internet Installation,
                Huawei & Ubiquiti Setup,
                Village Internet Project.
            </p>
        </div>

    </div>

    <!-- CONTACT -->
    <div class="section">

        <div class="section-title">
            Contact
        </div>

        <div class="card">
            <p>
                📧 sehudin872@gmail.com
            </p>
        </div>

        <div class="socials">

            <a href="#">
                💼
            </a>

            <a href="#">
                📸
            </a>

            <a href="#">
                💻
            </a>

            <a href="#">
                ▶
            </a>

        </div>

    </div>

    <!-- FOOTER -->
    <div class="footer">
        ⚡ Building Networks • Creating Solutions • Empowering Technology
    </div>

</div>

</div>

</body>
</html>
