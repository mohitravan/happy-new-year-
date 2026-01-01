<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy New Year 2026 - Rani</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500;700&family=Poppins:wght@400;600&family=Titan+One&display=swap" rel="stylesheet">
    <style>
        * {
            padding: 0;
            margin: 0;
            box-sizing: border-box;
        }

        :root {
            --color-bg: #1a0033;
            --color-pink: #ff66b2;
            --color-purple: #d946ef;
            --color-white: #fff;
            --color-black: #333;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #1a0033 0%, #2d1b4e 50%, #4a1b5e 100%);
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
            color: white;
        }

        #wrapper {
            position: relative;
            min-height: 100vh;
            overflow: hidden;
        }

        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: #ff99cc;
            border-radius: 50%;
            animation: twinkle 3s infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 1; }
        }

        .content {
            position: relative;
            width: 100%;
            display: flex;
            padding-top: 3rem;
            z-index: 2;
            min-height: 100vh;
        }

        .content .left,
        .content .right {
            position: relative;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        .content .left {
            width: 40%;
            padding: 20px;
        }

        .content .right {
            width: 60%;
            padding: 20px;
        }

        .title {
            position: relative;
            width: 100%;
            display: flex;
            justify-content: center;
            font-family: "Titan One", sans-serif;
            font-size: 3rem;
            flex-direction: column;
            perspective: 1000px;
        }

        .title .happy,
        .title .newyear {
            position: relative;
            text-shadow: 4px 4px var(--color-black),
                -4px 4px var(--color-black),
                4px -4px var(--color-black),
                -4px -4px var(--color-black),
                4px 8px 0 var(--color-black);
            font-weight: bold;
            display: flex;
            justify-content: center;
        }

        .title .happy {
            color: var(--color-pink);
        }

        .title .newyear {
            color: var(--color-purple);
        }

        .title .happy span,
        .title .newyear span {
            transform: translateY(50px);
            opacity: 0;
            visibility: hidden;
            animation: txtTranslateY 0.5s var(--t) forwards;
        }

        @keyframes txtTranslateY {
            100% {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }
        }

        .year-badge {
            display: inline-block;
            background: linear-gradient(135deg, var(--color-purple), var(--color-pink));
            color: white;
            padding: 15px 50px;
            border-radius: 50px;
            font-size: 2rem;
            font-weight: bold;
            margin-top: 20px;
            border: 4px solid var(--color-black);
            box-shadow: 0 5px 20px rgba(217, 70, 239, 0.5);
            animation: dateOfBirth 5s 4s forwards;
            transform: translateY(-100px);
            opacity: 0;
        }

        @keyframes dateOfBirth {
            to {
                transform: translateY(0px);
                opacity: 1;
                visibility: visible;
            }
        }

        .btn {
            transform: scale(0);
            animation: scaleCricle 2s 6s forwards ease-in-out;
        }

        @keyframes scaleCricle {
            0% {
                transform: scale(0);
            }
            10% {
                transform: scale(1.3);
            }
            20% {
                transform: scale(0.7);
            }
            30%, 100% {
                transform: scale(1);
            }
        }

        #btn__letter {
            position: relative;
            margin-top: 30px;
            background-color: var(--color-pink);
            outline: none;
            padding: 15px 30px;
            font-size: 1.2rem;
            border-radius: 50px;
            border: 3px solid var(--color-black);
            font-family: "Poppins", sans-serif;
            font-weight: bold;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            color: white;
            transition: all 0.5s ease-in-out;
        }

        #btn__letter:hover {
            background-color: var(--color-purple);
            transform: scale(1.1);
            box-shadow: 0 8px 30px rgba(217, 70, 239, 0.7);
        }

        #btn__letter i {
            margin-left: 10px;
        }

        .box__account {
            position: relative;
            transform: translateY(700px);
            animation: topBoxImage 3s 3s forwards ease-in;
        }

        @keyframes topBoxImage {
            to {
                transform: translateY(0);
            }
        }

        .image-container {
            position: relative;
            width: 350px;
            height: 350px;
            border-radius: 50%;
            overflow: hidden;
            border: 6px solid var(--color-black);
            background: linear-gradient(135deg, var(--color-purple), var(--color-pink));
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .image-container i {
            font-size: 10rem;
            color: white;
            opacity: 0.3;
        }

        .name {
            position: absolute;
            padding: 10px 30px;
            bottom: -20px;
            background: linear-gradient(135deg, var(--color-purple), var(--color-pink));
            border-radius: 50px;
            border: 3px solid var(--color-black);
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            font-weight: bold;
            color: white;
        }

        .floating-element {
            position: absolute;
            animation: float 4s ease-in-out infinite;
            font-size: 3rem;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
            }
            50% {
                transform: translateY(-30px) rotate(10deg);
            }
        }

        .champagne {
            top: 15%;
            left: 10%;
        }

        .confetti-icon {
            top: 25%;
            right: 15%;
        }

        .party-popper {
            bottom: 20%;
            left: 12%;
        }

        .sparkles {
            bottom: 30%;
            right: 10%;
        }

        .boxMail {
            position: fixed;
            background: rgba(0, 0, 0, 0.95);
            width: 100%;
            height: 100%;
            opacity: 0;
            top: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            transform: scale(0.3);
            visibility: hidden;
            transition: all 0.5s;
            z-index: 100;
        }

        .boxMail.active {
            opacity: 1;
            visibility: visible;
            transform: scale(1);
        }

        .boxMail-container {
            position: relative;
            width: 750px;
            height: 500px;
            display: flex;
            perspective: 2000px;
            transition: all 0.5s;
        }

        .boxMail-container:hover {
            transform: rotate(-5deg);
            filter: drop-shadow(0 0 20px var(--color-pink));
        }

        .boxMail-container:hover .card1 {
            transform: translate(-187px, -250px) rotateY(-140deg);
        }

        .card1,
        .card2 {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            border: 2px solid var(--color-black);
            border-radius: 15px;
        }

        .card1 {
            width: 50%;
            background: linear-gradient(135deg, var(--color-purple), var(--color-pink));
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            z-index: 1;
            transform-style: preserve-3d;
            transform-origin: left;
            transition: all 1s ease-in-out;
        }

        .card1 .userIcon {
            width: 100px;
            height: 100px;
            background-color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 3px solid white;
            margin-bottom: 20px;
        }

        .card1 .userIcon i {
            font-size: 3rem;
            color: var(--color-purple);
        }

        .card1 h3 {
            font-family: 'Dancing Script', cursive;
            font-size: 40px;
            text-transform: uppercase;
            text-align: center;
            letter-spacing: 3px;
            text-shadow: 0 0 10px white;
        }

        .card2 {
            width: 50%;
            background: linear-gradient(to right, #e0e0e0, #ffffff 30%);
            transform-style: preserve-3d;
            transform-origin: left;
        }

        .card2-content {
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--color-purple), var(--color-pink));
            transition: all 1s;
            overflow-y: auto;
            padding: 30px;
            color: white;
            border-radius: 15px;
        }

        .boxMail-container:hover .card2-content {
            transform: translate(20px, 20px);
            box-shadow: -5px -5px 15px rgba(0, 0, 0, 0.4);
        }

        .card2 h3 {
            font-family: 'Dancing Script', cursive;
            font-size: 35px;
            margin-bottom: 20px;
            text-shadow: 0 0 10px white;
        }

        .card2 p {
            font-family: 'Poppins', sans-serif;
            font-size: 18px;
            line-height: 1.8;
            text-align: justify;
        }

        .fa-xmark {
            position: fixed;
            top: 20px;
            right: 20px;
            font-size: 40px;
            cursor: pointer;
            color: white;
            z-index: 101;
            transition: transform 0.3s;
        }

        .fa-xmark:hover {
            transform: rotate(90deg);
        }

        @media (max-width: 768px) {
            .content {
                flex-direction: column;
            }

            .content .left,
            .content .right {
                width: 100%;
            }

            .title {
                font-size: 2rem;
            }

            .image-container {
                width: 250px;
                height: 250px;
            }

            .boxMail-container {
                width: 90%;
                height: 400px;
                flex-direction: column;
            }

            .card1,
            .card2 {
                width: 100%;
                height: 50%;
            }

            .boxMail-container:hover .card1 {
                transform: translate(-250px, -187px) rotateX(-140deg);
            }

            .card1 {
                transform-origin: top;
            }
        }
    </style>
</head>
<body>
    <div id="wrapper">
        <div class="stars" id="stars"></div>

        <div class="floating-element champagne">🥂</div>
        <div class="floating-element confetti-icon">🎊</div>
        <div class="floating-element party-popper">🎉</div>
        <div class="floating-element sparkles">✨</div>

        <div class="content">
            <div class="left">
                <div class="title">
                    <h1 class="happy">
                        <span style="--t: 0.5s;">H</span>
                        <span style="--t: 0.7s;">a</span>
                        <span style="--t: 0.9s;">p</span>
                        <span style="--t: 1.1s;">p</span>
                        <span style="--t: 1.3s;">y</span>
                    </h1>
                    <h1 class="newyear">
                        <span style="--t: 1.5s;">N</span>
                        <span style="--t: 1.7s;">e</span>
                        <span style="--t: 1.9s;">w</span>
                        <span style="--t: 2.1s;"> </span>
                        <span style="--t: 2.3s;">Y</span>
                        <span style="--t: 2.5s;">e</span>
                        <span style="--t: 2.7s;">a</span>
                        <span style="--t: 2.9s;">r</span>
                    </h1>
                </div>

                <div class="year-badge">
                    <i class="fas fa-calendar-star"></i> 2026
                </div>

                <div class="btn">
                    <button id="btn__letter">
                        Click Here Rani
                        <i class="fa-regular fa-envelope"></i>
                    </button>
                </div>
            </div>

            <div class="right">
                <div class="box__account">
                    <div class="image-container">
                        <i class="fas fa-user"></i>
                    </div>
                    <div class="name">
                        <i class="fa-solid fa-heart"></i>
                        Dear Rani
                        <i class="fa-solid fa-heart"></i>
                    </div>
                </div>
            </div>
        </div>

        <div class="boxMail">
            <i class="fa-solid fa-xmark"></i>
            <div class="boxMail-container">
                <div class="card1">
                    <div class="userIcon">
                        <i class="fas fa-star"></i>
                    </div>
                    <h3>To: Rani 💖</h3>
                </div>
                <div class="card2">
                    <div class="card2-content">
                        <h3>Happy New Year 2026! 🎉</h3>
                        <p>
                            Dear Rani,<br><br>
                            
                            As we step into this brand new year, I want to wish you all the happiness and success that life has to offer! 🌟<br><br>
                            
                            May 2026 bring you countless moments of joy, amazing opportunities, and the courage to chase all your dreams. You deserve all the wonderful things coming your way!<br><br>
                            
                            Thank you for being such an incredible friend. Here's to another year filled with laughter, adventures, and unforgettable memories together! 🥳<br><br>
                            
                            May this year be your best one yet! Keep shining bright like the star you are! ✨🌟<br><br>
                            
                            Cheers to new beginnings and endless possibilities!<br><br>
                            
                            With love and best wishes,<br>
                            Your Friend 💕
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Generate stars
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 150; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = Math.random() * 100 + '%';
            star.style.top = Math.random() * 100 + '%';
            star.style.animationDelay = Math.random() * 3 + 's';
            starsContainer.appendChild(star);
        }

        // Mail box functionality
        let mailBox = document.querySelector('#btn__letter');
        let boxmail = document.querySelector('.boxMail');
        let close = document.querySelector('.fa-xmark');

        mailBox.onclick = function() {
            boxmail.classList.add('active');
        }

        close.addEventListener('click', function() {
            boxmail.classList.remove('active');
        });

        // Close on outside click
        boxmail.addEventListener('click', function(e) {
            if (e.target === boxmail) {
                boxmail.classList.remove('active');
            }
        });
    </script>
</body>
</html>
