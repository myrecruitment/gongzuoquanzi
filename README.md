<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>居家行政助理招聘 | 兼职全职均可</title>
    <meta name="description" content="Marriott Bonvoy Hotels招聘居家行政助理，月薪RM5000-8000+，弹性工作时间，无需经验，免费培训">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, 'Helvetica Neue', Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .container {
            background: white;
            padding: 50px 40px;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
            text-align: center;
            max-width: 520px;
            width: 100%;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
            animation: fadeIn 0.8s ease-out;
        }

        .container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
        }

        .header {
            margin-bottom: 40px;
            animation: slideDown 0.6s ease-out;
        }

        .company-info {
            margin-bottom: 25px;
        }

        .company-badge {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 8px 20px;
            border-radius: 25px;
            font-size: 14px;
            font-weight: 600;
            letter-spacing: 0.5px;
            display: inline-block;
            margin-bottom: 12px;
            animation: popIn 0.5s ease-out;
        }

        .company-name {
            color: #2d3748;
            font-size: 24px;
            font-weight: 800;
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: 8px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        h1 {
            color: #1a202c;
            margin-bottom: 12px;
            font-size: 28px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .job-title {
            color: #667eea;
            font-size: 18px;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .subtitle {
            color: #718096;
            margin-bottom: 30px;
            font-size: 16px;
            font-weight: 400;
        }

        .job-highlights {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            grid-template-rows: repeat(2, 1fr);
            gap: 15px;
            margin-bottom: 25px;
            animation: fadeIn 0.8s 0.2s both;
        }

        .highlight-item {
            background: linear-gradient(135deg, #f7fafc, #edf2f7);
            padding: 20px 15px;
            border-radius: 12px;
            border: 1px solid #e2e8f0;
            transition: all 0.3s ease;
        }

        .highlight-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            border-color: #667eea;
        }

        .highlight-icon {
            font-size: 24px;
            margin-bottom: 8px;
            display: block;
        }

        .highlight-text {
            font-size: 14px;
            font-weight: 600;
            color: #2d3748;
        }

        .highlight-desc {
            font-size: 12px;
            color: #718096;
            margin-top: 4px;
        }

        .live-counter {
            background: linear-gradient(135deg, #f0fff4, #c6f6d5);
            color: #22543d;
            padding: 12px 20px;
            border-radius: 12px;
            margin-bottom: 20px;
            font-size: 14px;
            font-weight: 700;
            border: 2px solid #68d391;
            animation: counterPulse 1.5s infinite;
        }

        @keyframes counterPulse {
            0%, 100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(104, 211, 145, 0.4); }
            50% { transform: scale(1.02); box-shadow: 0 0 0 10px rgba(104, 211, 145, 0); }
        }

        .cta-section {
            margin-bottom: 25px;
            animation: fadeIn 0.8s 0.4s both;
            position: relative;
        }

        .cta-button {
            background: linear-gradient(135deg, #48bb78, #38a169);
            color: white;
            border: none;
            padding: 20px 40px;
            font-size: 20px;
            font-weight: 700;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            max-width: 350px;
            box-shadow: 0 8px 20px rgba(72, 187, 120, 0.3);
            position: relative;
            overflow: hidden;
            margin-bottom: 15px;
            animation: buttonGlow 2s infinite;
        }

        .salary-highlight {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 25px;
            border-radius: 16px;
            margin-bottom: 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(102, 126, 234, 0.5); }
            70% { box-shadow: 0 0 0 15px rgba(102, 126, 234, 0); }
            100% { box-shadow: 0 0 0 0 rgba(102, 126, 234, 0); }
        }

        .salary-amount {
            font-size: 32px;
            font-weight: 700;
            margin-bottom: 8px;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }

        .salary-desc {
            font-size: 16px;
            opacity: 0.9;
        }

        .urgency-note {
            background: linear-gradient(135deg, #fed7d7, #fbb6ce);
            color: #c53030;
            padding: 15px 20px;
            border-radius: 12px;
            margin-bottom: 20px;
            font-size: 14px;
            font-weight: 600;
            border-left: 4px solid #e53e3e;
            position: relative;
            overflow: hidden;
            animation: slideUp 0.5s 0.6s both;
        }

        @keyframes buttonGlow {
            0%, 100% { box-shadow: 0 8px 20px rgba(72, 187, 120, 0.3); }
            50% { box-shadow: 0 8px 30px rgba(72, 187, 120, 0.6); }
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(72, 187, 120, 0.5);
        }

        .status {
            margin-top: 20px;
            padding: 12px 20px;
            border-radius: 8px;
            font-weight: 500;
            display: none;
        }

        .status.success {
            background: #c6f6d5;
            color: #22543d;
            border: 1px solid #9ae6b4;
        }

        .status.error {
            background: #fed7d7;
            color: #c53030;
            border: 1px solid #feb2b2;
        }

        .fallback-container {
            margin-top: 20px;
            background: #fefcbf;
            padding: 15px;
            border-radius: 8px;
            border: 1px solid #f6e05e;
            display: none;
            animation: fadeIn 0.5s;
        }

        .fallback-link {
            display: block;
            margin-top: 10px;
            word-break: break-all;
            color: #744210;
            text-decoration: none;
            font-weight: 500;
        }

        .fallback-link:hover {
            text-decoration: underline;
        }

        .footer {
            text-align: center;
            color: #a0aec0;
            font-size: 14px;
            margin-top: 25px;
            padding-top: 20px;
            border-top: 1px solid #e2e8f0;
            animation: fadeIn 0.8s 0.8s both;
        }

        .trust-indicators {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
            flex-wrap: wrap;
            animation: fadeIn 0.8s 0.7s both;
        }

        .trust-item {
            display: flex;
            align-items: center;
            gap: 5px;
            color: #718096;
            font-size: 12px;
            background: #f7fafc;
            padding: 6px 12px;
            border-radius: 15px;
            border: 1px solid #e2e8f0;
            transition: all 0.3s ease;
        }

        .trust-item:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        /* 新增样式 */
        .wechat-warning {
            background: #ffecb3;
            color: #5d4037;
            padding: 12px;
            border-radius: 8px;
            margin: 15px 0;
            text-align: center;
            border-left: 4px solid #ffa000;
            animation: slideUp 0.5s 0.6s both;
        }
        
        .multiple-cta {
            display: flex;
            gap: 10px;
            justify-content: center;
            margin-top: 15px;
        }
        
        .mini-cta {
            background: linear-gradient(135deg, #4299e1, #3182ce);
            color: white;
            border: none;
            padding: 12px 20px;
            font-size: 14px;
            font-weight: 600;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            flex: 1;
            max-width: 160px;
            box-shadow: 0 4px 10px rgba(66, 153, 225, 0.3);
        }
        
        .mini-cta:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(66, 153, 225, 0.4);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes slideDown {
            from { opacity: 0; transform: translateY(-30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes popIn {
            0% { opacity: 0; transform: scale(0.8); }
            70% { transform: scale(1.1); }
            100% { opacity: 1; transform: scale(1); }
        }
        
        @keyframes slideUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 480px) {
            .container {
                padding: 30px 20px;
                margin: 10px;
            }
            
            h1 {
                font-size: 24px;
            }
            
            .job-title {
                font-size: 16px;
            }
            
            .subtitle {
                font-size: 14px;
            }

            .company-info {
                text-align: center;
            }

            .job-highlights {
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: repeat(2, 1fr);
                gap: 12px;
            }

            .salary-amount {
                font-size: 28px;
            }

            .trust-indicators {
                gap: 8px;
            }

            .trust-item {
                font-size: 11px;
                padding: 4px 8px;
            }
            
            .cta-button {
                padding: 18px 30px;
                font-size: 18px;
            }
            
            .multiple-cta {
                flex-direction: column;
                gap: 8px;
            }
            
            .mini-cta {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="company-info">
                <div class="company-badge">五星级酒店集团</div>
                <div class="company-name">Marriott Bonvoy Hotels</div>
            </div>
            <h1>招聘居家行政助理</h1>
            <div class="job-title">兼职/全职 • 居家办公 • 弹性时间</div>
            <p class="subtitle">无需经验，提供完整培训，欢迎宝妈、学生、上班族</p>
        </div>

        <div class="job-highlights">
            <div class="highlight-item">
                <span class="highlight-icon">💰</span>
                <div class="highlight-text">RM5000-8000+</div>
                <div class="highlight-desc">月收入范围</div>
            </div>
            <div class="highlight-item">
                <span class="highlight-icon">🏠</span>
                <div class="highlight-text">居家办公</div>
                <div class="highlight-desc">无需通勤</div>
            </div>
            <div class="highlight-item">
                <span class="highlight-icon">⏰</span>
                <div class="highlight-text">3-4小时/天</div>
                <div class="highlight-desc">弹性工作时间</div>
            </div>
            <div class="highlight-item">
                <span class="highlight-icon">📚</span>
                <div class="highlight-text">免费培训</div>
                <div class="highlight-desc">零基础可学</div>
            </div>
        </div>

        <div class="live-counter" id="liveCounter">
            🔥 实时：已有 <span id="counterNumber">18</span> 人正在咨询！
        </div>

        <!-- 微信环境提示 -->
        <div class="wechat-warning" id="wechatWarning" style="display: none;">
            <strong>⚠️ 微信提示：</strong> 
            请点击右上角...选择"在浏览器打开"以正常跳转WhatsApp
        </div>

        <!-- 主CTA按钮 -->
        <div class="cta-section">
            <button class="cta-button whatsapp-btn" data-source="main-cta">
                💬 立即开始咨询
            </button>
            
            <div class="multiple-cta">
                <button class="mini-cta whatsapp-btn" data-source="cta-1">
                    📱 手机咨询
                </button>
                <button class="mini-cta whatsapp-btn" data-source="cta-2">
                    💻 电脑咨询
                </button>
                <button class="mini-cta whatsapp-btn" data-source="cta-3">
                    ⏱️ 快速申请
                </button>
            </div>
        </div>

        <div class="salary-highlight">
            <div class="salary-amount">RM 6,500</div>
            <div class="salary-desc">平均月收入 • 多劳多得 • 上不封顶</div>
        </div>

        <div class="urgency-note">
            ⚡ 紧急招聘：今日截止！已有<span id="applicantCount">26</span>人投递简历，仅剩<span id="remainingCount">3</span>个名额！
        </div>

        <div class="trust-indicators">
            <div class="trust-item">
                <span>🏆</span>
                <span>五星酒店</span>
            </div>
            <div class="trust-item">
                <span>🛡️</span>
                <span>正规企业</span>
            </div>
            <div class="trust-item">
                <span>⭐</span>
                <span>真实岗位</span>
            </div>
            <div class="trust-item">
                <span>🔒</span>
                <span>信息保密</span>
            </div>
            <div class="trust-item">
                <span>✅</span>
                <span>免费咨询</span>
            </div>
        </div>

        <div class="status" id="status"></div>
        
        <div class="fallback-container" id="fallbackContainer">
            <p>您的浏览器阻止了自动跳转，请手动点击下方链接：</p>
            <a href="#" class="fallback-link" id="whatsappFallbackLink" target="_blank"></a>
        </div>

        <div class="footer">
            <p>点击任意按钮将通过WhatsApp与我们的专业招聘顾问联系</p>
            <p style="margin-top: 8px; font-size: 12px;">我们承诺：100%免费咨询，不收取任何费用</p>
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
        const PHONE_NUMBER = '+60148665044';
        const WHATSAPP_PROTOCOL_LINK = `whatsapp://send?phone=${PHONE_NUMBER}`;
        
        // 检测微信环境
        function isWeChatBrowser() {
            return /MicroMessenger/i.test(navigator.userAgent);
        }
        
        // 显示微信警告
        if (isWeChatBrowser()) {
            document.getElementById('wechatWarning').style.display = 'block';
        }
        
        // 快速更新的实时计数器
        function updateLiveCounter() {
            const counterElement = document.getElementById('counterNumber');
            const baseCount = 18;
            const randomIncrease = Math.floor(Math.random() * 5) + 1; // 1-5的随机增长
            const newCount = baseCount + randomIncrease;
            
            if (counterElement) {
                counterElement.textContent = newCount;
            }
        }
        
        // 更新申请人计数
        function updateApplicantCount() {
            const applicantElement = document.getElementById('applicantCount');
            const remainingElement = document.getElementById('remainingCount');
            
            if (applicantElement && remainingElement) {
                const currentApplicants = parseInt(applicantElement.textContent);
                const currentRemaining = parseInt(remainingElement.textContent);
                
                // 随机增加1-3个申请人，减少1-2个名额
                const newApplicants = currentApplicants + Math.floor(Math.random() * 3) + 1;
                const newRemaining = Math.max(0, currentRemaining - Math.floor(Math.random() * 2) - 1);
                
                applicantElement.textContent = newApplicants;
                remainingElement.textContent = newRemaining;
                
                // 如果名额用完，重置
                if (newRemaining <= 0) {
                    setTimeout(() => {
                        applicantElement.textContent = 30;
                        remainingElement.textContent = 5;
                    }, 5000);
                }
            }
        }
        
        // 每10秒更新一次计数器
        setInterval(updateLiveCounter, 10000);
        setInterval(updateApplicantCount, 15000);
        
        // 简化追踪函数 - 只保留Contact事件
        function trackConsultationClick(buttonSource) {
            if (typeof fbq === 'undefined') return;
            
            try {
                fbq('track', 'Contact', {
                    content_name: 'WhatsApp点击',
                    content_category: '用户联系',
                    value: 8.00,
                    currency: 'USD'
                });
            } catch (error) {
                console.error('追踪事件失败:', error);
            }
        }
        
        // 显示状态信息
        function showStatus(message, type) {
            const statusDiv = document.getElementById('status');
            statusDiv.textContent = message;
            statusDiv.className = `status ${type}`;
            statusDiv.style.display = 'block';
            
            setTimeout(() => {
                statusDiv.style.display = 'none';
            }, 1500);
        }
        
        // 显示备用方案
        function showFallbackOption() {
            const fallbackContainer = document.getElementById('fallbackContainer');
            const fallbackLink = document.getElementById('whatsappFallbackLink');
            
            fallbackLink.href = WHATSAPP_LINK;
            fallbackLink.textContent = WHATSAPP_LINK;
            fallbackContainer.style.display = 'block';
        }
        
        // 主要联系函数 - 极速跳转版本
        function contactWhatsApp(event) {
            const button = event.currentTarget;
            const buttonSource = button.getAttribute('data-source') || 'unknown';
            
            // 立即追踪
            trackConsultationClick(buttonSource);
            
            // 短暂禁用按钮防止连续点击
            const originalText = button.innerHTML;
            button.disabled = true;
            button.innerHTML = '🚀 跳转中...';
            
            // 显示加载状态
            showStatus('正在连接招聘顾问...', 'success');
            
            try {
                // 策略1: 尝试协议链接（移动端）
                const protocolLink = document.createElement('a');
                protocolLink.href = WHATSAPP_PROTOCOL_LINK;
                protocolLink.style.display = 'none';
                document.body.appendChild(protocolLink);
                protocolLink.click();
                document.body.removeChild(protocolLink);
                
                // 策略2: 同时打开网页版
                setTimeout(() => {
                    window.open(WHATSAPP_LINK, '_blank');
                }, 100);
                
            } catch (error) {
                // 策略3: 显示备用链接
                showFallbackOption();
            }
            
            // 快速恢复按钮（0.5秒后）
            setTimeout(() => {
                button.disabled = false;
                button.innerHTML = originalText;
            }, 500);
        }
        
        // 页面加载完成
        window.addEventListener('load', function() {
            // 绑定所有咨询按钮
            document.querySelectorAll('.whatsapp-btn').forEach(button => {
                button.addEventListener('click', contactWhatsApp);
            });
            
            // 设置备用链接
            document.getElementById('whatsappFallbackLink').href = WHATSAPP_LINK;
            document.getElementById('whatsappFallbackLink').textContent = WHATSAPP_LINK;
            
            // 快速更新计数器
            updateLiveCounter();
            updateApplicantCount();
        });
    </script>
</body>
</html>
