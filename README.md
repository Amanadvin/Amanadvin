<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smiley Face</title>
    <style>
        .smiley {
            position: relative;
            width: 200px;
            height: 200px;
            background-color: yellow;
            border-radius: 50%;
            margin: 50px auto;
        }
        .smiley::before,
        .smiley::after {
            content: '';
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: black;
            border-radius: 50%;
        }
        .smiley::before {
            top: 50px;
            left: 50px;
        }
        .smiley::after {
            top: 50px;
            right: 50px;
        }
        .smile {
            position: absolute;
            bottom: 40px;
            left: 50%;
            width: 120px;
            height: 60px;
            border: 5px solid black;
            border-radius: 0 0 60px 60px;
            transform: translateX(-50%);
        }
    </style>
</head>
<body>
    <div class="smiley">
        <div class="smile"></div>
    </div>
</body>
</html>
