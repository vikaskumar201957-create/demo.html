<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GameHub UI Demo</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    color: white;
    font-family: Arial, sans-serif;
    background:
        radial-gradient(circle at 15% 15%, #39258a55, transparent 30%),
        radial-gradient(circle at 85% 30%, #087c9250, transparent 28%),
        linear-gradient(145deg, #070812, #0d1020 55%, #080910);
}

.nav {
    max-width: 1150px;
    margin: auto;
    padding: 22px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 21px;
    font-weight: bold;
}

.logo span {
    color: #22d3ee;
}

.navlinks {
    display: flex;
    gap: 22px;
    color: #9ca3bd;
    font-size: 14px;
}

.navlinks b {
    color: white;
}

.hero {
    max-width: 1150px;
    margin: 55px auto 35px;
    padding: 0 22px;
}

.badge {
    display: inline-block;
    padding: 7px 12px;
    border: 1px solid #7c5cff66;
    background: #7c5cff22;
    border-radius: 30px;
    color: #c9bfff;
    font-size: 12px;
}

h1 {
    font-size: clamp(42px, 7vw, 76px);
    line-height: 1;
    margin: 18px 0;
    max-width: 760px;
}

.hero p {
    color: #9ca3bd;
    font-size: 17px;
    line-height: 1.6;
    max-width: 650px;
}

.cta {
    margin-top: 20px;
    padding: 13px 20px;
    border: 0;
    border-radius: 13px;
    color: white;
    font-weight: bold;
    background: linear-gradient(135deg, #7c5cff, #9b7cff);
    box-shadow: 0 12px 30px #7c5cff55;
    cursor: pointer;
}

.section {
    max-width: 1150px;
    margin: 40px auto 70px;
    padding: 0 22px;
}

.section-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 18px;
}

.section-head h2 {
    margin: 0;
}

.section-head span {
    color: #9ca3bd;
    font-size: 13px;
}

.grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
}

.card {
    position: relative;
    min-height: 220px;
    padding: 22px;
    border-radius: 22px;
    border: 1px solid #ffffff18;
    background: #171a2bb8;
    backdrop-filter: blur(15px);
    transition: .25s;
    overflow: hidden;
}

.card:hover {
    transform: translateY(-7px);
    border-color: #7c5cff88;
    box-shadow: 0 20px 50px #00000055;
}

.icon {
    font-size: 42px;
}

.card h3 {
    margin: 15px 0 8px;
    font-size: 20px;
}

.card p {
    color: #9ca3bd;
    font-size: 13px;
    line-height: 1.5;
}

.play {
    position: absolute;
    right: 18px;
    bottom: 18px;
    padding: 8px 12px;
    border: 1px solid #ffffff18;
    border-radius: 10px;
    background: #ffffff0d;
    color: white;
}

.stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin-top: 16px;
}

.stat {
    padding: 18px;
    border-radius: 18px;
    border: 1px solid #ffffff12;
    background: #ffffff08;
}

.stat small {
    color: #9ca3bd;
}

.stat strong {
    display: block;
    font-size: 25px;
    margin-top: 7px;
}

@media (max-width: 760px) {

    .navlinks {
        display: none;
    }

    .grid {
        grid-template-columns: 1fr;
    }

    .stats {
        grid-template-columns: 1fr;
    }

    .hero {
        margin-top: 30px;
    }
}
</style>
</head>

<body>

<nav class="nav">

    <div class="logo">
        GAME<span>HUB</span> ✦
    </div>

    <div class="navlinks">
        <b>Home</b>
        <span>Games</span>
        <span>Leaderboard</span>
        <span>About</span>
    </div>

</nav>

<section class="hero">

    <span class="badge">● ONLINE • UI CONCEPT</span>

    <h1>
        Play something<br>
        you'll remember.
    </h1>

    <p>
        A modern gaming dashboard built with HTML,
        CSS and JavaScript.
    </p>

    <button class="cta">
        Explore Games →
    </button>

</section>

<section class="section">

    <div class="section-head">
        <h2>Featured Games</h2>
        <span>3 available</span>
    </div>

    <div class="grid">

        <div class="card">
            <div class="icon">✊</div>

            <h3>
                Rock Paper Scissors
            </h3>

            <p>
                Classic quick-match game with
                score and animated feedback.
            </p>

            <button class="play">
                Play ↗
            </button>
        </div>

        <div class="card">
            <div class="icon">⭕</div>

            <h3>
                Tic-Tac-Toe
            </h3>

            <p>
                Challenge the computer or a friend
                in a modern board.
            </p>

            <button class="play">
                Soon
            </button>
        </div>

        <div class="card">
            <div class="icon">🐍</div>

            <h3>
                Snake
            </h3>

            <p>
                Classic arcade gameplay with
                score tracking.
            </p>

            <button class="play">
                Soon
            </button>
        </div>

    </div>

    <div class="stats">

        <div class="stat">
            <small>GAMES PLAYED</small>
            <strong>1,248</strong>
        </div>

        <div class="stat">
            <small>HIGH SCORE</small>
            <strong>8,420</strong>
        </div>

        <div class="stat">
            <small>PLAY TIME</small>
            <strong>14h 32m</strong>
        </div>

    </div>

</section>

</body>
</html>
