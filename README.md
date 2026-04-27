# hww26
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <title>HW23 - 圖片樣式練習</title>
    <style>
        body {
            font-family: sans-serif;
            text-align: center;
            background-color: #f6f6f6;
            padding: 40px;
        }

        .gallery {
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin-top: 30px;
        }

        /* 基礎樣式：框線與內距 (參考您的 Thumbnail 範例) */
        img {
            border: 1px solid #ddd;
            background: white;
            padding: 5px;
        }

        /* 左邊：艾菲爾鐵塔 (圓角 18px / 不變形) */
        .left-tower {
            width: 300px;
            height: 300px;
            border-radius: 18px;
            object-fit: cover; /* 保持比例不變形 */
        }

        /* 中間：地球 (正圓形) */
        .center-earth {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
        }

        /* 右邊：艾菲爾鐵塔 (寬度 33% / 形變練習) */
        .right-tower {
            width: 33%;
            height: 300px;
            object-fit: fill; /* 故意製造擠壓感，讓鐵塔看起來變瘦 */
        }

        p {
            font-size: 13px;
            color: #666;
            margin-top: 10px;
        }
    </style>
</head>
<body>

    <h2>CSS Styling Images (HW23)</h2>

    <div class="gallery">
        <div>
            <img src="paris.jpg" class="left-tower" alt="Paris Cover">
            <p>Radius: 18px (No Distortion)</p>
        </div>

        <div>
            <img src="earth.jpg" class="center-earth" alt="Earth Circle">
            <p>Circle (150x150)</p>
        </div>

        <div>
            <img src="Paris1.jpg" class="right-tower" alt="Paris Distorted">
            <p>Width: 33% / Height: 300px (Fill)</p>
        </div>
    </div>

</body>
</html>
