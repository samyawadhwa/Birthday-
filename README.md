# Birthday-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Happy Birthday Pushkar</title>
    <style>
        /* Modern Reset */
        * { box-sizing: border-box; margin: 0; padding: 0; }

        body, html {
            width: 100%;
            height: 100%;
            background-color: #000;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        /* Full Screen Floral Border */
        .floral-border {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            pointer-events: none;
            z-index: 10;
            border: 20px solid transparent;
            /* Using a cleaner flower pattern */
            border-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Ctext y='50' font-size='40'%3E🌸%3C/text%3E%3Ctext x='50' y='90' font-size='40'%3E🌺%3C/text%3E%3C/svg%3E") 30 round;
        }

        .container {
            text-align: center;
            z-index: 5;
            padding: 20px;
        }

        /* Appear Animation for Text */
        .fade-up {
            opacity: 0;
            transform: translateY(30px);
            animation: appear 1.2s ease-out forwards;
        }

        .line-1 {
            color: #ffffff;
            font-size: 2rem;
            font-weight: 300;
            margin-bottom: 5px;
        }

        .line-2 {
            color: #ff4081;
            font-size: 4.5rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 3px;
            animation-delay: 0.6s; /* Pushkar appears slightly later */
            text-shadow: 0 0 15px rgba(255, 64, 129, 0.5);
        }

        @keyframes appear {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Center Glow */
        .glow {
            position: absolute;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255, 64, 129, 0.1) 0%, rgba(0,0,0,0) 80%);
            z-index: 1;
        }
    </style>
</head>
<body>

    <div class="floral-border"></div>
    <div class="glow"></div>

    <div class="container">
        <div class="line-1 fade-up">Happiest Birthday</div>
        <div class="line-2 fade-up">Pushkar</div>
    </div>

</body>
</html>
