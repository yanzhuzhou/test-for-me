<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>老婆我爱你</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;}
body{width:100vw;min-height:100vh;background:linear-gradient(120deg,#ff9a9e 0%,#fecfef 50%,#fecfef 100%);display:flex;justify-content:center;align-items:center;font-family:"Microsoft YaHei",sans-serif;overflow:hidden;flex-direction:column;}
.text{font-size:42px;font-weight:bold;color:#ff4d8f;text-align:center;line-height:1.6;animation:fadeIn 2s ease,float 3s infinite ease-in-out;text-shadow:0 0 10px rgba(255,255,255,0.8);}
@keyframes float{0%,100%{transform:translateY(0px);}50%{transform:translateY(-15px);}}
@keyframes fadeIn{from{opacity:0;}to{opacity:1;}}
.heart{position:absolute;color:#ff4d8f;font-size:20px;animation:heartMove 5s linear infinite;z-index:-1;}
@keyframes heartMove{0%{transform:translateY(100vh) rotate(0deg);opacity:1;}100%{transform:translateY(-100vh) rotate(720deg);opacity:0;}}
</style>
</head>
<body>
<div class="text">老婆老婆我爱你<br>一起一起不分离</div>
<script>
function createHeart(){const heart=document.createElement('div');heart.innerHTML='❤️';heart.classList.add('heart');heart.style.left=Math.random()*100+'vw';heart.style.fontSize=Math.random()*20+10+'px';heart.style.animationDuration=Math.random()*3+3+'s';document.body.appendChild(heart);setTimeout(()=>{heart.remove();},5000);}
setInterval(createHeart,300);
</script>
</body>
</html>
