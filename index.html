<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>应用跳转页面</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Microsoft YaHei', Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .container {
            max-width: 400px;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        
        .title {
            font-size: 24px;
            font-weight: bold;
            color: #333;
            margin-bottom: 30px;
        }
        
        .app-button {
            display: block;
            width: 100%;
            padding: 15px 20px;
            margin: 15px 0;
            border: none;
            border-radius: 12px;
            font-size: 16px;
            font-weight: bold;
            text-decoration: none;
            color: white;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .app-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
        }
        
        .xiaohongshu {
            background: linear-gradient(45deg, #ff2442, #ff6b6b);
        }
        
        .douyin {
            background: linear-gradient(45deg, #000000, #333333);
        }
        
        .wechat {
            background: linear-gradient(45deg, #07c160, #38a169);
        }
        
        .icon {
            margin-right: 8px;
            font-size: 18px;
        }
        
        .tips {
            margin-top: 30px;
            font-size: 12px;
            color: #666;
            line-height: 1.6;
        }
        
        .error-msg {
            display: none;
            margin-top: 15px;
            padding: 10px;
            background: #fff3cd;
            border: 1px solid #ffeaa7;
            border-radius: 8px;
            color: #856404;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 class="title">选择要打开的应用</h1>
        
        <a href="javascript:void(0)" class="app-button xiaohongshu" onclick="openXiaohongshu()">
            <span class="icon">🌹</span>
            打开小红书
        </a>
        
        <a href="javascript:void(0)" class="app-button douyin" onclick="openDouyin()">
            <span class="icon">🎵</span>
            打开抖音
        </a>
        
        <a href="javascript:void(0)" class="app-button wechat" onclick="shareToMoments()">
            <span class="icon">💬</span>
            分享到朋友圈
        </a>
        
        <div id="errorMsg" class="error-msg"></div>
        
        <div class="tips">
            <p>• 点击按钮将尝试打开对应的应用</p>
            <p>• 如果应用未安装，将提示下载</p>
            <p>• 朋友圈功能将调用微信分享</p>
        </div>
    </div>

    <script>
        function openXiaohongshu() {
            // 尝试打开小红书APP
            const xiaohongshuScheme = 'xhsdiscover://';
            const xiaohongshuWeb = 'https://www.xiaohongshu.com/';
            
            // 创建隐藏的iframe尝试打开APP
            const iframe = document.createElement('iframe');
            iframe.style.display = 'none';
            iframe.src = xiaohongshuScheme;
            document.body.appendChild(iframe);
            
            // 如果APP未打开，则跳转到网页版
            setTimeout(() => {
                window.location.href = xiaohongshuWeb;
                document.body.removeChild(iframe);
            }, 2000);
        }
        
        function openDouyin() {
            // 尝试打开抖音APP
            const douyinScheme = 'snssdk1128://';
            const douyinWeb = 'https://www.douyin.com/';
            
            // 创建隐藏的iframe尝试打开APP
            const iframe = document.createElement('iframe');
            iframe.style.display = 'none';
            iframe.src = douyinScheme;
            document.body.appendChild(iframe);
            
            // 如果APP未打开，则跳转到网页版
            setTimeout(() => {
                window.location.href = douyinWeb;
                document.body.removeChild(iframe);
            }, 2000);
        }
        
        function shareToMoments() {
            // 检查是否在微信浏览器中
            const isWechat = /micromessenger/i.test(navigator.userAgent);
            
            if (isWechat) {
                // 在微信中，提示用户手动分享
                showError('请点击右上角"..."按钮，选择"分享到朋友圈"');
                
                // 也可以尝试调用微信JS-SDK分享功能（需要配置）
                if (typeof wx !== 'undefined') {
                    wx.ready(function() {
                        wx.onMenuShareTimeline({
                            title: '应用跳转页面',
                            link: window.location.href,
                            imgUrl: '',
                            success: function () {
                                showError('分享成功！');
                            },
                            cancel: function () {
                                showError('用户取消分享');
                            }
                        });
                    });
                }
            } else {
                showError('请在微信中打开此页面以使用朋友圈分享功能');
            }
        }
        
        function showError(message) {
            const errorDiv = document.getElementById('errorMsg');
            errorDiv.textContent = message;
            errorDiv.style.display = 'block';
            
            // 3秒后隐藏提示
            setTimeout(() => {
                errorDiv.style.display = 'none';
            }, 3000);
        }
        
        // 页面加载完成后的初始化
        window.onload = function() {
            // 检查是否在微信浏览器中
            const isWechat = /micromessenger/i.test(navigator.userAgent);
            if (!isWechat) {
                showError('建议在微信中打开此页面以获得最佳体验');
            }
        };
    </script>
</body>
</html>
