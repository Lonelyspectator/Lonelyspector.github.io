<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <title>一个孤独的个人网站</title>
    <style type="text/css">
        body {
            background-color: #000000; 
            color: #ffffff; 
            font-family: "宋体", Arial, sans-serif; 
            text-align: center; 
            margin-top: 15%; 
            padding: 0 20px; 
            line-height: 1.8;
        }
        h1 {
            color: #00ff00; 
        }
        #lang-btn {
            background-color: #333333;
            color: #00ff00;
            border: 1px solid #00ff00;
            padding: 5px 15px;
            font-size: 14px;
            cursor: pointer;
            margin-bottom: 30px;
        }
        /* 默认隐藏英文区域 */
        #english-content {
            display: none; 
        }
    </style>
</head>
<body>

    <!-- 语言切换按钮 -->
    <button id="lang-btn" onclick="switchLanguage()">Switch to English / 切换中文</button>

    <!-- 中文内容区域 -->
    <div id="chinese-content">
        <h1>哦，好吧</h1>

        <p>看样子你发现一个非常孤独的个人网站。</p>
        <p>虽然这里现在非常单调，而且只有这些。</p>
        <p>但是你知道的，个人网站也是有特别之处的。</p>
        <p>那么你们就当这是一个新的、每个人都能进入的小房子。哦，对了，这是我第1个网站</p>
        
        <!-- 这是你刚加的新内容 -->
        <p>这次有一个小更新，这个网站现在有两个语言模式，一个是中文一个是英文。说实话，我以后还打算更新这个网页。虽然估计又是漫长的时间...</p>
        <p>看到这里的人，祝你们每天开心！ ( ^ v ^ )</p>
        
        <p>:)</p>
    </div>

    <!-- 英文内容区域 -->
    <div id="english-content">
        <h1>Oh, alright.</h1>

        <p>Looks like you've found a very lonely personal website.</p>
        <p>Although it is very plain right now, and has nothing but these words.</p>
        <p>But you know, personal websites have their own special charm.</p>
        <p>So just treat it as a new, little house that everyone can enter. Oh, right, this is my first website.</p>
        
        <!-- 这是上面那段中文的英文翻译 -->
        <p>There's a small update: this site now has two language modes, Chinese and English. To be honest, I plan to keep updating this website in the future. Though it might take a long time...</p>
        <p>To anyone reading this, I wish you happiness every day! ( ^ v ^ )</p>
        
        <p>:)</p>
    </div>

    <!-- 切换语言的魔法代码 -->
    <script type="text/javascript">
        var currentLang = 0; 

        function switchLanguage() {
            var chineseBox = document.getElementById("chinese-content");
            var englishBox = document.getElementById("english-content");
            
            if (currentLang == 0) {
                chineseBox.style.display = "none";
                englishBox.style.display = "block";
                currentLang = 1; 
            } else {
                englishBox.style.display = "none";
                chineseBox.style.display = "block";
                currentLang = 0; 
            }
        }
    </script>

</body>
</html>