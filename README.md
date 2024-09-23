# mini-netflixx
trabalhode escola
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini Netflix</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #141414;
            color: #fff;
            margin: 0;
            padding: 20px;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .video-card {
            position: relative;
            width: 300px;
            height: 170px;
            overflow: hidden;
            border-radius: 8px;
            transition: transform 0.3s;
        }
        .video-card:hover {
            transform: scale(1.05);
        }
        .video-card iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s;
        }
        .video-card:hover .overlay {
            opacity: 1;
        }
        .overlay-text {
            font-size: 20px;
            text-align: center;
        }
    </style>
</head>
<body>

    <h1>Mini Netflix</h1>
    <div class="container">
        <div class="video-card">
            <iframe src="https://www.youtube.com/embed/E8MtS5Mloxk?si=JUbCUkTwEpDR4d9j" allowfullscreen></iframe>
            <div class="overlay">
                <div class="overlay-text">Assistir Video 1</div>
            </div>
        </div>
        <div class="video-card">
            <iframe src="https://www.youtube.com/embed/X7e3qJXe7_w?si=6YQXv6pjjYbrmmSc" allowfullscreen></iframe>
            <div class="overlay">
                <div class="overlay-text">Assistir Video 2</div>
            </div>
        </div>
    </div>

</body>
</html>
