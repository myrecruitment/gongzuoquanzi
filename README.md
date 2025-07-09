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
            margin-bottom: 40px;
            font-size: 16px;
            font-weight: 400;
        }

        .job-highlights {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            grid-template-rows: repeat(2, 1fr);
            gap: 15px;
            margin-bottom: 35px;
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

        .salary-highlight::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: shimmer 3s ease-in-out infinite;
        }

        @keyframes shimmer {
            0%, 100% { opacity: 0; }
            50% { opacity: 1; }
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

        .cta-section {
            margin-bottom: 25px;
            animation: fadeIn 0.8s 0.4s both;
        }

        .cta-button {
            background: linear-gradient(135deg, #48bb78, #38a169);
            color: white;
            border: none;
            padding: 18px 40px;
            font-size: 18px;
            font-weight: 700;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            max-width: 300px;
            box-shadow: 0 8px 20px rgba(72, 187, 120, 0.3);
            position: relative;
            overflow: hidden;
            margin-bottom: 15px;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }

        .cta-button:hover::before {
            left: 100%;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(72, 187, 120, 0.4);
        }

        .cta-button:active {
            transform: translateY(-1px);
        }

        .cta-button:disabled {
            opacity: 0.7;
            transform: none;
            cursor: not-allowed;
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

        .urgency-note::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: urgencyShine 2s infinite;
        }

        @keyframes urgencyShine {
            0% { left: -100%; }
            100% { left: 100%; }
        }

        .intent-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 1000;
        }

        .intent-modal.show {
            display: flex;
        }

        .intent-content {
            background: white;
            padding: 30px;
            border-radius: 16px;
            text-align: center;
            max-width: 400px;
            width: 90%;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
            animation: modalSlideIn 0.5s ease-out;
        }

        @keyframes modalSlideIn {
            from { transform: scale(0.8) translateY(-50px); opacity: 0; }
            to { transform: scale(1) translateY(0); opacity: 1; }
        }

        .intent-content h3 {
            color: #2d3748;
            margin-bottom: 15px;
            font-size: 20px;
        }

        .intent-content p {
            color: #718096;
            margin-bottom: 25px;
            font-size: 14px;
        }

        .intent-buttons {
            display: flex;
            gap: 10px;
            justify-content: center;
        }

        .intent-btn {
            padding: 12px 24px;
            border: none;
            border-radius: 25px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .intent-btn.primary {
            background: linear-gradient(135deg, #48bb78, #38a169);
            color: white;
        }

        .intent-btn.secondary {
            background: #f7fafc;
            color: #718096;
            border: 1px solid #e2e8f0;
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

        .live-counter {
            background: #f0fff4;
            color: #22543d;
            padding: 10px 15px;
            border-radius: 8px;
            margin-bottom: 15px;
            font-size: 13px;
            font-weight: 600;
            border: 1px solid #68d391;
            animation: counterPulse 2s infinite;
        }

        @keyframes counterPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.02); }
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
                padding: 16px 30px;
                font-size: 16px;
            }

            .intent-buttons {
                flex-direction: column;
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
            🔥 今日已有 <span id="counterNumber">12</span> 人咨询，剩余名额有限
        </div>

        <!-- 唯一的CTA按钮 -->
        <div class="cta-section">
            <button class="cta-button whatsapp-btn" data-source="highlights-section">
                💬 立即咨询详情
            </button>
        </div>

        <div class="salary-highlight">
            <div class="salary-amount">RM 6,500</div>
            <div class="salary-desc">平均月收入 • 多劳多得 • 上不封顶</div>
        </div>

        <div class="urgency-note">
            🔥 限时招聘：本月仅招收15名，已有8人确认面试，剩余名额有限！
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
            <p>点击按钮将通过WhatsApp与我们的专业招聘顾问联系</p>
            <p style="margin-top: 8px; font-size: 12px;">我们承诺：100%免费咨询，不收取任何费用</p>
        </div>
    </div>

    <!-- 意图确认弹窗 -->
    <div class="intent-modal" id="intentModal">
        <div class="intent-content">
            <h3>📞 确认咨询意向</h3>
            <p>您确定要了解这个工作机会吗？我们的招聘顾问将为您详细介绍岗位信息和薪资待遇。</p>
            <div class="intent-buttons">
                <button class="intent-btn primary" onclick="confirmIntent()">确定咨询</button>
                <button class="intent-btn secondary" onclick="cancelIntent()">再想想</button>
            </div>
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
        
        // 状态管理
        let hasTrackedLead = false;
        let userClickCount = 0;
        let pageStartTime = Date.now();
        let currentButton = null;
        let currentButtonSource = null;
        
        // 实时计数器更新
        function updateLiveCounter() {
            const counterElement = document.getElementById('counterNumber');
            const baseCount = 12;
            const randomIncrease = Math.floor(Math.random() * 3); // 0-2的随机增长
            const newCount = baseCount + randomIncrease;
            
            if (counterElement) {
                counterElement.textContent = newCount;
            }
        }
        
        // 每30秒更新一次计数器
        setInterval(updateLiveCounter, 30000);
        
        // 延迟追踪函数 - 高质量转化
        function trackConsultationClick(buttonSource) {
            console.log('🎯 延迟追踪咨询点击 - 来源:', buttonSource);
            
            // 防止重复追踪
            if (hasTrackedLead) {
                console.log('⚠️ 已追踪过Lead，跳过');
                return;
            }
            
            if (typeof fbq === 'undefined') {
                console.error('❌ Facebook Pixel 未加载');
                return;
            }
            
            try {
                // 只有确认意图后才发送Lead事件
                fbq('track', 'Lead', {
                    content_name: 'WhatsApp联系',
                    content_category: '高质量咨询',
                    value: 20.00,
                    currency: 'USD'
                });
                
                hasTrackedLead = true;
                console.log('✅ 高质量Lead事件已发送');
                
                // 发送Contact作为补充数据
                fbq('track', 'Contact', {
                    content_name: 'WhatsApp确认点击',
                    content_category: '真实意图'
                });
                
            } catch (error) {
                console.error('❌ 追踪事件失败:', error);
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
            }, 3000);
        }
        
        // 显示备用方案
        function showFallbackOption() {
            showStatus('跳转失败，请手动点击下方链接', 'error');
            
            const fallbackContainer = document.getElementById('fallbackContainer');
            const fallbackLink = document.getElementById('whatsappFallbackLink');
            
            fallbackLink.href = WHATSAPP_LINK;
            fallbackLink.textContent = WHATSAPP_LINK;
            fallbackContainer.style.display = 'block';
        }
        
        // 执行WhatsApp跳转
        function executeWhatsAppRedirect() {
            const isMobile = /iPhone|iPad|iPod|Android|webOS|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent);
            
            try {
                if (isMobile) {
                    console.log('📱 移动设备 - 尝试协议链接');
                    
                    // 创建隐藏iframe尝试协议链接
                    const iframe = document.createElement('iframe');
                    iframe.style.display = 'none';
                    iframe.src = WHATSAPP_PROTOCOL_LINK;
                    document.body.appendChild(iframe);
                    
                    // 设置回退机制
                    setTimeout(() => {
                        if (document.hasFocus()) {
                            console.log('🔄 回退到网页版');
                            window.open(WHATSAPP_LINK, '_blank');
                        }
                    }, 1000);
                    
                    // 清理iframe
                    setTimeout(() => {
                        if (document.body.contains(iframe)) {
                            document.body.removeChild(iframe);
                        }
                    }, 3000);
                } else {
                    console.log('💻 桌面设备 - 网页版');
                    window.open(WHATSAPP_LINK, '_blank');
                }
                
                // 延迟3秒后追踪Lead事件（确保用户真的进入了WhatsApp）
                setTimeout(() => {
                    trackConsultationClick(currentButtonSource);
                }, 3000);
                
            } catch (error) {
                console.log('❌ 跳转失败:', error);
                showFallbackOption();
            }
        }
        
        // 确认意图
        function confirmIntent() {
            console.log('✅ 用户确认咨询意图');
            
            // 隐藏弹窗
            document.getElementById('intentModal').classList.remove('show');
            
            // 显示状态
            showStatus('正在连接招聘顾问...', 'success');
            
            // 执行跳转
            executeWhatsAppRedirect();
            
            // 恢复按钮状态
            if (currentButton) {
                setTimeout(() => {
                    currentButton.disabled = false;
                    currentButton.innerHTML = '💬 立即咨询详情';
                }, 3000);
            }
        }
        
        // 取消意图
        function cancelIntent() {
            console.log('❌ 用户取消咨询');
            
            // 追踪取消行为
            try {
                fbq('track', 'ViewContent', {
                    content_name: '取消咨询意图',
                    content_category: '用户犹豫'
                });
            } catch (error) {
                console.log('取消追踪失败:', error);
            }
            
            // 隐藏弹窗
            document.getElementById('intentModal').classList.remove('show');
            
            // 恢复按钮状态
            if (currentButton) {
                currentButton.disabled = false;
                currentButton.innerHTML = '💬 立即咨询详情';
            }
            
            showStatus('如有疑问，随时可以再次咨询', 'error');
        }
        
        // 主要联系函数 - 意图检测优化
        function contactWhatsApp(event) {
            const button = event.target;
            const buttonSource = button.getAttribute('data-source') || 'unknown';
            const timeOnPage = Date.now() - pageStartTime;
            
            console.log('👆 用户点击咨询按钮');
            console.log('⏱️ 页面停留时间:', Math.round(timeOnPage/1000), '秒');
            
            if (button.disabled) {
                console.log('⚠️ 按钮已禁用');
                return;
            }
            
            // 保存当前按钮引用
            currentButton = button;
            currentButtonSource = buttonSource;
            userClickCount++;
            
            // 禁用按钮
            button.disabled = true;
            button.innerHTML = '🤔 请确认意向...';
            
            // 意图检测逻辑
            if (timeOnPage < 8000) {
                // 停留时间少于8秒，显示确认弹窗
                console.log('⚠️ 页面停留时间较短，显示意图确认');
                document.getElementById('intentModal').classList.add('show');
            } else {
                // 停留时间足够，直接跳转
                console.log('✅ 页面停留时间充足，直接执行');
                button.innerHTML = '
