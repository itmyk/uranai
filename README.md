<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>今日の運勢占</title>
    <style>
        body { text-align: center; font-family: sans-serif; padding-top: 50px; }
        #result { font-size: 3rem; font-weight: bold; color: #e74c3c; margin: 20px; }
    </style>
</head>
<body>
    <h1>あなたの今日の運勢は…</h1>
    <div id="result">？？？</div>
    <button onclick="location.reload()">もう一度引く</button>

    <script>
        const results = ["大吉", "中吉", "小吉", "吉", "末吉", "凶"];
        const random = results[Math.floor(Math.random() * results.length)];
        document.getElementById("result").innerText = random;
    </script>
</body>
</html>
