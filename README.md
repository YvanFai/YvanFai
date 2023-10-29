<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome</title>

    <style>
        body{
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: #000;
        }

        h2{
            position: relative;
            margin: 20px 0 0;
            font-size: 4em;
            font-weight: 900;
            color: #fff;
            z-index: 1;
            overflow: hidden;
        }

        h2::before{
            content: '';
            position: absolute;
            left: 110%;
            width: 120%;
            height: 100%;
            background: linear-gradient(90deg , transparent 0% , #000 5% , #000 100%);
            animation: animate 5.5s linear forwards;
            animation-delay: 2s;
        }

        @keyframes animate{
            0%{
                left: 110%;
            }
            100%{
                left: -20%;
            }
        }

        h2 span{
            color: #ff022c;
        }

        video{
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 2;
            pointer-events: none;
            mix-blend-mode: screen;
        }

    </style>

</head>
<body>
    <video src = "https://www.youtube.com/watch?v=PP0Os0UvMCs" , muted = "" , autoplay = ""></video>
    <h2> <span>We</span>lcome <span>to</span> my <span>Git</span>hub</h2>
</body>
</html>
