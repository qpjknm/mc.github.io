<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EmpireCraft服务器</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f9;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .container {
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            max-width: 600px;
            width: 100%;
            text-align: center;
        }
        h1 {
            color: #4CAF50;
        }
        .button {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px 0;
            background-color: #4CAF50;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #45a049;
        }
        .contact {
            margin-top: 20px;
        }
        .robot {
            width: 100px;
            height: 150px;
            background-color: #4CAF50;
            border-radius: 50px;
            margin: 20px auto;
            position: relative;
            cursor: pointer;
            transition: transform 0.3s, background-color 0.3s;
            animation: float 3s infinite ease-in-out, blink 2s infinite;
        }
        .robot::before {
            content: '';
            position: absolute;
            width: 40px;
            height: 20px;
            background-color: white;
            border-radius: 20px;
            top: 60px;
            left: 30px;
        }
        .robot::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: white;
            border-radius: 50%;
            top: 90px;
            left: 40px;
        }
        .robot:hover {
            transform: translateY(-5px);
            background-color: #45a049;
        }
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
        }
        @keyframes blink {
            0%, 100% {
                transform: scaleY(1);
            }
            50% {
                transform: scaleY(0.8);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>EmpireCraft服务器</h1>
        <p>cn带土制作的一个简单的网页</p>
        <h2>欢迎加入EmpireCraft服务器</h2>
        <p>这是一个公益免费的服务器，欢迎加入！</p>
        <p>作者：cn带土</p>
        <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=luXVF0M8gV4KUUMOf43U-SbXotM4Wuzr&authKey=%2Fqu0W5eiLQG%2FpPFGoLtWCwfnmDywEQFd7t9Cfx%2Bp4FLojKr6oRUUO8A%2F%2FUgtvkl%2F&noverify=0&group_code=747086715" class="button" id="joinQQGroup">点击加入QQ群聊</a>
        <div class="contact">
            <p>QQ群号：747086715</p>
            <p>需要赞助的加QQ：875752110</p>
        </div>
        <div class="robot" id="robot"></div>
    </div>

    <script>
        const robot = document.getElementById('robot');
        const joinQQGroup = document.getElementById('joinQQGroup');

        robot.addEventListener('click', () => {
            window.open(joinQQGroup.href, '_blank'); // 在新标签页中打开链接
        });
    </script>
</body>
</html>
