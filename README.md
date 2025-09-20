<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EmpireCraft服务器</title>
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
