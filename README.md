<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>居家助理招聘</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, 'Helvetica Neue', Arial, sans-serif;
            background: #f8fafc;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            line-height: 1.6;
        }

        .container {
            background: white;
            padding: 60px 50px;
            border-radius: 16px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            text-align: center;
            max-width: 480px;
            width: 100%;
            border: 1px solid #e5e7eb;
        }

        .logo {
            width: 64px;
            height: 64px;
            margin: 0 auto 32px;
            background: linear-gradient(135deg, #10b981, #059669);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            color: white;
            font-weight: 600;
        }

        h1 {
            color: #1f2937;
            margin-bottom: 16px;
            font-size: 32px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .subtitle {
            color: #6b7280;
            margin-bottom: 48px;
            font-size: 18px;
            font-weight: 400;
            max-width: 400px;
            margin-left: auto;
            margin-right: auto;
        }

        .features {
            margin-bottom: 48px;
            text-align: left;
        }

        .feature {
            display: flex;
            align-items: flex-start;
            margin-bottom: 24px;
            padding: 20px;
            background: #f9fafb;
            border-radius: 12px;
            border: 1px solid #f3f4f6;
            transition: all 0.2s ease;
        }

        .feature:hover {
            background: #f0fdf4;
            border-color: #d1fae5;
        }

        .feature-icon {
            width: 20px;
            height: 20px;
            margin-right: 16px;
            color: #10b981;
            font-size: 16px;
            margin-top: 2px;
        }

        .feature-text {
            color: #374151;
            font-size: 16px;
            font-weight: 500;
        }

        .cta-button {
            background: linear-gradient(135deg, #10b981, #059669);
            color: white;
            border: none;
            padding: 16px 32px;
            font-size: 18px;
            font-weight: 600;
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.2s ease;
            width: 100%;
            box-shadow: 0 4px 12px rgba(16, 185, 129, 0.25);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 16px rgba(16, 185, 129, 0.35);
        }

        .cta-button:active {
            transform: translateY(0);
        }

        .footer {
            margin-top: 32px;
            color: #9ca3af;
            font-size: 14px;
        }

        .status {
            margin-top: 24px;
            padding: 12px 20px;
            border-radius: 8px;
            font-weight: 500;
            display: none;
        }

        .status.success {
            background: #ecfdf5;
            color: #065f46;
            border: 1px solid #a7f3d0;
        }
        
        .status.error {
            background: #fef2f2;
            color: #991b1b;
            border: 1px solid #fecaca;
        }
        
        .status-link {
            color: #065f46;
            text-decoration: underline;
            font-weight: 600;
            cursor: pointer;
        }
        
        .status-link:hover {
            color: #047857;
        }
        
        .fallback-container {
            margin-top: 20px;
            background: #fffbeb;
            padding: 15px;
            border-radius: 8px;
            border: 1px solid #fde68a;
            display: none;
        }
        
        .fallback-link {
            display: block;
            margin-top: 10px;
            word-break: break-all;
            color: #065f46;
            text-decoration: none;
            font-weight: 500;
        }
        
        .fallback-link:hover {
            text-decoration: underline;
        }

        @media (max-width: 480px) {
            .container {
                padding: 40px 30px;
            }
            
            h1 {
                font-size: 28px;
            }
            
            .subtitle {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="logo">💼</div>
        <h1>居家助理招聘</h1>
        <p class="subtitle">有无经验都可以申请，提供全面培训</p>
        
        <div class="features">
            <div class="feature">
                <div class="feature-icon">✨</div>
                <div class="feature-text">月入可达RM5000-RM8000+</div>
            </div>
            <div class="feature">
                <div class="feature-icon">🎯</div>
                <div class="feature-text">每日灵活3-4小时工作</div>
            </div>
            <div class="feature">
                <div class="feature-icon">⚡</div>
                <div class="feature-text">无需经验，文凭</div>
            </div>
        </div>

        <button class="cta-button" id="whatsappButton">
            开始咨询
        </button>

        <div class="status" id="status"></div>
        
        <div class="fallback-container" id="fallbackContainer">
            <p>您的浏览器阻止了自动跳转，请手动点击下方链接：</p>
            <a href="#" class="fallback-link" id="whatsappFallbackLink" target="_blank"></a>
        </div>

        <div class="footer">
            <p>点击按钮将通过WhatsApp与我们的招聘顾问取得联系</p>
        </div>
    </div>

    <!-- Facebook Pixel Code -->
    <script>
        !function(f,b,e,v,n,t,s)
        {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
        n.callMethod.apply(n,arguments):n.queue.push(arguments)};
        if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
        n.queue=[];t=b.createElement(e);t.async=!0;
        t.src=v;s=b.getElementsByTagName(e)[0];
        s.parentNode.insertBefore(t,s)}(window, document,'script',
        'https://connect.facebook.net/en_US/fbevents.js');

        // Facebook Pixel 初始化
        fbq('init', '623059780216649'); 
        fbq('track', 'PageView');
    </script>
    <noscript>
        <img height="1" width="1" style="display:none" 
             src="https://www.facebook.com/tr?id=623059780216649&ev=PageView&noscript=1"/>
    </noscript>

    <script>
        // 配置
        const WHATSAPP_LINK = 'https://wa.link/gongzuquanzi';
        
        // 状态管理
        let whatsappClicked = false;
        
        // 显示状态信息
        function showStatus(message, type, autoHide = true) {
            const statusDiv = document.getElementById('status');
            statusDiv.textContent = message;
            statusDiv.className = `status ${type}`;
            statusDiv.style.display = 'block';
            
            if (autoHide) {
                setTimeout(() => {
                    statusDiv.style.display = 'none';
                }, 3000);
            }
        }
        
        // 追踪WhatsApp点击 - 核心追踪函数
        function trackWhatsAppClick() {
            if (typeof fbq === 'undefined') {
                console.error('❌ Facebook Pixel 未加载');
                return;
            }
            
            try {
                // Lead事件 - 主要转化追踪
                fbq('track', 'Lead', {
                    content_name: 'WhatsApp联系',
                    content_category: '招聘咨询',
                    value: 20.00,
                    currency: 'USD'
                });
                
                console.log('✅ WhatsApp点击事件已追踪');
                
            } catch (error) {
                console.error('❌ 追踪事件失败:', error);
            }
        }
        
        // 优化后的WhatsApp联系函数
        function contactWhatsApp() {
            console.log('🚀 用户点击WhatsApp联系');
            
            // 防止重复点击
            if (whatsappClicked) {
                console.log('⚠️ 重复点击，忽略');
                return;
            }
            whatsappClicked = true;
            
            // 追踪WhatsApp点击事件
            trackWhatsAppClick();
            
            // 显示加载状态
            showStatus('正在跳转到WhatsApp...', 'success');
            
            // 方法1: 尝试直接在当前窗口打开（移动端友好）
            try {
                window.location.href = WHATSAPP_LINK;
                return;
            } catch (e) {
                console.log('方法1失败', e);
            }
            
            // 方法2: 尝试在新窗口打开（桌面端友好）
            try {
                const newWindow = window.open(WHATSAPP_LINK, '_blank');
                if (newWindow && !newWindow.closed) {
                    return;
                }
            } catch (e) {
                console.log('方法2失败', e);
            }
            
            // 方法3: 使用a标签模拟点击
            try {
                const link = document.createElement('a');
                link.href = WHATSAPP_LINK;
                link.target = '_blank';
                link.rel = 'noopener noreferrer';
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
                return;
            } catch (e) {
                console.log('方法3失败', e);
            }
            
            // 如果所有方法都失败，显示备用方案
            showFallbackOption();
        }
        
        // 显示备用方案
        function showFallbackOption() {
            console.log('显示WhatsApp备用方案');
            
            // 显示错误状态
            showStatus('跳转失败，请手动打开WhatsApp', 'error', false);
            
            // 显示备用链接容器
            const fallbackContainer = document.getElementById('fallbackContainer');
            const fallbackLink = document.getElementById('whatsappFallbackLink');
            
            fallbackLink.href = WHATSAPP_LINK;
            fallbackLink.textContent = WHATSAPP_LINK;
            fallbackContainer.style.display = 'block';
        }
        
        // 页面加载完成
        window.addEventListener('load', function() {
            console.log('📱 招聘页面加载完成');
            
            // 添加事件监听器
            document.getElementById('whatsappButton').addEventListener('click', contactWhatsApp);
            
            // 验证Pixel状态
            if (typeof fbq !== 'undefined') {
                console.log('✅ Facebook Pixel 已正确加载');
            } else {
                console.error('❌ Facebook Pixel 加载失败');
            }
        });
        
        // 监听页面离开 - 检测WhatsApp使用
        window.addEventListener('beforeunload', function() {
            if (whatsappClicked) {
                console.log('📊 用户在点击WhatsApp后离开页面');
            }
        });
        
        // 监听窗口失焦 - 可能在使用WhatsApp
        window.addEventListener('blur', function() {
            if (whatsappClicked) {
                console.log('📱 窗口失焦 - 用户可能在使用WhatsApp');
            }
        });
    </script>
</body>
</html>
