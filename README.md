<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Lyrics Vibes Team | Member Profile</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600;700&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

body{
    min-height:100vh;
    background:
        radial-gradient(circle at 50% -10%, #214d91 0%, #0b2855 32%, #06152f 65%, #020a18 100%);
    color:#fff;
    font-family:'Montserrat',sans-serif;
    padding:22px 14px 30px;
}

.page{
    width:100%;
    max-width:480px;
    margin:auto;
}

/* =========================
   HEADER
========================= */

.header{
    text-align:center;
    margin-bottom:18px;
}

.header-line{
    width:48px;
    height:2px;
    background:#d9ad32;
    margin:0 auto 10px;
    border-radius:20px;
    box-shadow:0 0 9px rgba(217,173,50,.45);
}

.team-name{
    font-family:'Cinzel',serif;
    color:#e5ba45;
    font-size:clamp(21px,6vw,29px);
    font-weight:700;
    letter-spacing:1.2px;
    line-height:1.2;
}

.subtitle{
    margin-top:6px;
    color:#cfd8e8;
    font-size:9px;
    font-weight:500;
    letter-spacing:2.5px;
}

/* =========================
   MAIN CARD
========================= */

.card{
    position:relative;
    background:
        linear-gradient(
            145deg,
            rgba(11,39,80,.96),
            rgba(4,20,43,.98)
        );
    border:1px solid rgba(217,173,50,.72);
    border