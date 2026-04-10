<!DOCTYPE html>   < !DOCTYPE html><!DOCTYPE html>   < !DOCTYPE html>   < !DOCTYPE html>
<html lang="zh-CN">   < css长= " zh-CN" ><html lang="zh-CN">   < css长= " zh-CN" >
<head>   < head>   “标题”。
    <meta charset="UTF-8">   <meta charset   字符集="UTF-8"   "UTF-8">< meta charset   字符集=" UTF-8" >   <  UTF-8"   " UTF-8" >
    <meta name="viewport" content="width=device-width, initial-scale=1.0"><meta name="viewport" content="width=device-width, initial-scale=1.0"><meta name   名字="viewport"   "viewport" content="width=device-width, initial-scale=1.0"><meta name   名字="viewport"   "viewport" content="width=device-width, initial-scale=1.0">
    <title>老婆我爱你</title>   < title> Honey, I love you. /title>< title> Honey, I love you. /title>   < title> Honey, I love you. /title>
    <style>   < style>   “风格”
        * {
            margin: 0;   保证金:0;
            padding: 0;   填充:0;
            box-sizing: border-box;   盒模型尺寸计算方式：内容、内边距和边框的总和决定元素的尺寸
        }

        body {   身体{
            width: 100vw;
            min-height: 100vh;   最小高度:100 vh;min-height: 100vh;   Minimum height: 100vh;
            background: linear-gradient(120deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);背景：线性渐变（120 度，#ff9a9e 0%，#fecfef 50%，#fecfef 100%）；background: linear-gradient(120deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%); Background: Linear gradient (120 degrees, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);
            display: flex;   显示:flex;display: flex;   display: flex;
            justify-content: center;   居中对齐；justify-content: center;   Centered alignment;
            align-items: center;   align-items： 居中；align-items： 居中；
            font-family: "Microsoft YaHei", sans-serif;font-family: "Microsoft YaHei", sans-serif;font-family: "Microsoft YaHei", sans-serif;font-family: "Microsoft YaHei", sans-serif;
            overflow: hidden;   溢出:隐藏;overflow: hidden;   Overflow: Hidden;
            flex-direction: column;   flex-direction: column；  翻译为中文：主轴方向为垂直方向flex-direction: column;   "flex-direction: column" 翻译为中文：主轴方向为垂直方向

翻译成英文：The main axis direction is vertical.
        }

        /* 主文字样式 */
        .text {   ．文本{
            font-size: 42px;   字体大小:42 px;font-size: 42px;   Font size: 42 px;
            font-weight: bold;   粗细:大胆的;font-weight: bold;   Thickness: Bold;
            color: #ff4d8f;   颜色:# ff4d8f;color: #ff4d8f;   Color: #ff4d8f;
            text-align: center;   text-align:中心;文本对齐：居中； 文本对齐：中心；
            line-height: 1.6;   行高:1.6;
            animation: fadeIn 2s ease, float 3s infinite ease-in-out;动画：淡入 2 秒缓动，浮动 3 秒无限缓动；
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.8);文本阴影：0 0 10 像素 rgba(255, 255, 255， 0.8)；
        }

        /* 动画：浮动 */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }0%，100% { transform: translateY(0px); }}
            50% { transform: translateY(-15px); }50% 时 { 翻译 Y 轴(-15  }}
        }

        /* 动画：渐入 */
        @keyframes fadeIn {
            from { opacity: 0; }从 { 不 0；}
            to { opacity: 1; }到{透明度：1；}
        }

        /* 爱心飘动样式 */
        .heart {   ．心{
            position: absolute;   位置:绝对的;
            color: #ff4d8f;   颜色:# ff4d8f;color: #ff4d8f;   Color: #ff4d8f;
            font-size: 20px;   字体大小:20 px;
            animation: heartMove 5s linear infinite;动画：心形移动 5 秒 线性 无限循环；
            z-index: -1;   z - index: 1;
        }

        @keyframes heartMove {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 1;   透明度:1;
            }
            100% {
                transform: translateY(-100vh) rotate(720deg);
                opacity: 0;   透明度:0;
            }
        }
    </style>   < / style>
</head>   < / head>

<body>   < body>
    <div class="text">   <div class="text">
        老婆老婆我爱你<br>
        一起一起不分离
    </div>   < / div>

    <script>   < script>
        // 自动飘爱心
        function createHeart() {   function createHeart() {  创建爱心函数
            const heart = document.createElement('div');const heart = document.createElement('div')； 

// 直接翻译为中文：
const 心形 = document.createElement
            heart.innerHTML = '❤️';
            heart.classList.add('heart');
            
            // 随机大小、位置、速度
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.fontSize = Math.random() * 20 + 10 + 'px';
            heart.style.animationDuration = Math.random() * 3 + 3 + 's';heart.style.animationDuration = Math.random() * 3 + 's';
            
            document.body.appendChild(heart);文档主体追加子元素心形；
            
            // 5秒后移除
            setTimeout(() => {   setTimeout(() => {
                heart.remove();
            }, 5000);
        }

        // 每隔0.3秒飘一个爱心
        setInterval(createHeart, 300);
    </script>   < / script>
</body>   < / body>
</html>   < / html>
