<!DOCTYPE html>
<html lang="cn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <meta name="description" content="艾达艾 | adAI PPT生成器是一个永久免费的基于百度文心一言AI的ppt生成工具，用户只需输入需求，AI就能一键全自动生成高质量的PPT。">
    <meta name="keywords" content="AI PPT, chatgpt ppt, PPT生成器, AI PPT生成器">
    <title>艾达艾 | adAI PPT生成器,一个永久免费的基于ai的ppt生成器，ai一键生成ppt工具。</title>
    <link rel="stylesheet" href="./css/bootstrap.min.css">
    <style>
        body {
            background: url("/background.jpg") no-repeat center center fixed;
            background-size: cover;
            color: white;
        }
        .form-control, .btn {
            color: white;
        }
        .btn:hover {
            background-color: white;
            color: #65BC7B;
            border-color: white;
        }
        .navbar-toggler-icon {
        background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(255, 255, 255, 1)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
}

        .btn {
            background: url("/background.jpg") no-repeat center center fixed;
            background-size: cover;
            border-color: white;
            height: 50px;
        }
        .form-control {
            background-color: rgba(128, 0, 128, 0.7);
            border: none;
            border-radius: 10px;
        }
        #yonghutopic {
            padding-top: 13px;
            padding-left: 25px;
            min-height: 60px;
            background-color: rgba(255, 255, 255, 0.7); /* 30% 透明度 */
            color: black;
            border-width: 2px;
            border-color: transparent;
            outline: none;
}

        #yonghutopic::placeholder {
            color: #00000; /* 你可以使用你想要的任何颜色值 */
        }

        #formOptions {
            display: flex;
            justify-content: flex-start;
            align-items: center;
            margin-bottom: 1rem;
            margin-top: -15px;
        }
        #formOptions label {
            font-size: 0.8rem;
            color: rgba(255, 255, 255, 0.7);
            margin-right: 10px;
        }
        .navbar, .navbar-brand, .navbar-nav, .nav-link {
            color: white !important;
            background: url("/background.jpg") no-repeat center center fixed;
            background-size: cover;
        }
        @media (max-width: 768px) {
            #formOptions {
                flex-direction: row;
            }
        }
        #yuyan, #moban {
            background: url("/background.jpg") no-repeat center center fixed;
            background-color: rgb(107, 57,234);
            background-size: cover;
            border: #fff;
            color: #fff;
        }
        #yuyan option:hover, #moban option:hover {
            background: url("/background.jpg") no-repeat center center fixed;
            background-size: cover;;
        }
         /* Other CSS */
        #scrollingText {
        margin-bottom: 20px; /* 靠下一点 */
        font-size: 1rem; /* 字体大小可以根据需要进行调整 */
        color: #ffffff4d; /* 字体颜色 */
        }

        #adContainer {
            width: 100%; /* Set the width of the ad container */
            height: auto; /* Set the height of the ad container */
            margin: 20px auto; /* Center the ad container and add some margin on the top and bottom */
        }
        @media (max-width: 768px) {
            #adCarousel {
                /* 适应小屏幕的样式调整 */
                max-width: 100%; /* 确保轮播不会超出屏幕宽度 */
                height: auto; /* 自动调整高度 */
                overflow: hidden; /* 防止内容溢出 */
            }
        
            #adCarousel .carousel-item {
                display: flex; /* 使用flex布局确保内容居中 */
                justify-content: center; /* 水平居中 */
                align-items: center; /* 垂直居中 */
            }
        
            #adCarousel img {
                width: 100%; /* 图片宽度自适应 */
                height: auto; /* 高度自动 */
            }
            
            .carousel-control-prev, .carousel-control-next {
                /* 如果需要，可以调整控制按钮的样式 */
            }
        }
        /* Footer styles */
        /* 添加一些样式来装饰友情链接 */
        .footer .friend-links {
            margin: 20px 0; /* 添加一些上下的边距 */
        }
        .footer .friend-links h3 {
            font-size: 1.2em; /* 为标题设置一个合适的字体大小 */
            margin-bottom: 10px; /* 添加一些标题和链接之间的边距 */
        }
        .footer .friend-links ul {
            list-style-type: none; /* 去掉列表前的默认的点标记 */
            padding: 0; /* 去掉默认的padding */
        }
        .footer .friend-links ul li {
            display: inline-block; /* 使链接在一行内显示 */
            margin-right: 10px; /* 添加一些链接之间的边距 */
        }
        .footer .friend-links ul li a {
            color: white; /* 设置链接的颜色 */
            text-decoration: none; /* 去掉链接下的下划线 */
        }
        .footer .friend-links ul li a:hover {
            color: #cccccc; /* 当鼠标悬浮在链接上时，改变其颜色 */
        }

        .footer {
            color: white; /* Change footer text color to white */
            background: url("/background.jpg") no-repeat center center fixed;
            background-size: cover; /* Change footer background to match the rest of the site */
        }
        
        
    </style>
    <script src="./jquery-3.4.1.min.js"></script>
    <script src="./js/bootstrap.min.js"></script>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light">
        <a class="navbar-brand" href="#">
            <img src="logowhite.png" width="200" height="50" alt="logo">
        </a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="/index.html">首页</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/about.html">关于</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/help.html">帮助</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/contact.html">联系</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/ad.html">广告招商</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/tzr.html">投资人</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="/updates.html">更新日志</a>
                </li>
            </ul>
        </div>
    </nav>
    <div class="container mt-4">
        <h1 class="text-center" style="margin-top: 130px;margin-bottom: 50px;">AI PPT生成器</h1>
        <!-- AI PPT生成器标题下面添加一个新的div，用来显示滚动的句子 -->
        
        <div class="row justify-content-center"> <!-- 使用Bootstrap的 justify-content-center 类来使 topic 居中 -->
            <div class="col-lg-8"> <!-- 将lg改为8以增大topic的宽度 -->
                <form id="pptAddForm">
                    <div class="form-group">
                        <textarea class="form-control" id="yonghutopic" rows="6" placeholder="输入你对ppt制作的要求..." required></textarea>
                    </div>
                    <div id="formOptions">
                        <div class="form-group">
                            <select class="form-control" id="yuyan" required>
                                <option value="1">中文</option>
                                <option value="2">英文</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <select class="form-control" id="moban" required>
                                <option value="2">经典深色背景</option>
                                <option value="3">温馨波浪背景</option>
                                <option value="4">彩虹波浪背景</option>
                                <option value="1">经典浅色背景</option>
                                <option value="5">百度飞桨大赛背景</option>
                            </select>
                        </div>
                    </div>
                    <button type="submit" class="btn btn-primary btn-block" id="generateButton">一键生成PPT</button>
                    <br/>
                    <!--<h6 class="text-center" style="color: white;">提交后切勿关闭页面！</h6>                   -->
                    <!--<h6 class="text-center" style="color: white;">建议在电脑上使用，手机上如果无法生成建议更换浏览器尝试</h6>-->


                </form>
            </div>
        </div>
        <div id="scrollingText" class="text-center"></div>
    </div>
    <script src="main.js"></script>

    <!-- Footer -->
    <footer class="footer">
    <div class="container text-center">
        <!-- 添加一个新的div或section来容纳友情链接 -->
        <!--<div class="friend-links">-->
        <!--    <h4>友情链接</h4>-->
        <!--    <ul>-->
        <!--        <li><a href="https://ai.digilifeform.com">AI免费机器人聊天</a></li>-->
        <!--        <li><a href="https://www.antdanceai.com">wordpress + AI免费机器人聊天文章自动生成发布工具</a></li>-->
        <!--        <li><a href="https://www.digilifeform.com">ai数字生命定制</a></li>-->
        <!--        <li><a href="https://www.adaippt.com">huang145 AI PPT</a></li>-->
                <!-- 更多链接... -->
        <!--    </ul>-->
        <!--</div>-->
        <span class="text-muted">© 2024 huang145AI 版权所有.</span>
        <br/>
        <span class="text-muted">特别鸣谢114514</span>
    </div>
    </footer>

</body>
</html>
