<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Help TJ Become an Amazing Dad! 👶✨</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-gradient: linear-gradient(135deg, #ff6b9d, #c44569, #f8b500, #feca57);
            --secondary-gradient: linear-gradient(135deg, #667eea, #764ba2, #f093fb, #f5576c);
            --success-gradient: linear-gradient(135deg, #4facfe, #00f2fe);
            --warm-gradient: linear-gradient(135deg, #ffecd2, #fcb69f);
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(45deg, #ff9a9e, #fecfef, #fecfef, #ff9a9e);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            min-height: 100vh;
            overflow-x: hidden;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        @keyframes sparkle {
            0%, 100% { opacity: 0; transform: scale(0); }
            50% { opacity: 1; transform: scale(1); }
        }

        @keyframes slideIn {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .sparkles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .sparkle {
            position: absolute;
            width: 6px;
            height: 6px;
            background: #fff;
            border-radius: 50%;
            animation: sparkle 3s infinite;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 2;
        }

        header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 40px;
            margin-bottom: 30px;
            text-align: center;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            animation: slideIn 1s ease, float 6s ease-in-out infinite;
        }

        .logo {
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-size: 3.5em;
            font-weight: 800;
            margin-bottom: 15px;
            animation: pulse 2s infinite;
        }

        .tagline {
            color: #666;
            font-size: 1.3em;
            font-weight: 300;
        }

        .main-content {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 30px;
            margin-bottom: 30px;
        }

        @media (max-width: 768px) {
            .main-content {
                grid-template-columns: 1fr;
            }
        }

        .campaign-section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            animation: slideIn 1.2s ease;
        }

        .campaign-title {
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-size: 2.8em;
            font-weight: 800;
            margin-bottom: 30px;
            text-align: center;
            animation: pulse 3s infinite;
        }

        .hero-section {
            background: var(--warm-gradient);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero-section::before {
            content: '👶💖✨';
            position: absolute;
            top: -20px;
            right: -20px;
            font-size: 3em;
            opacity: 0.3;
            animation: float 4s ease-in-out infinite;
        }

        .campaign-image {
            width: 100%;
            height: 350px;
            background: var(--secondary-gradient);
            border-radius: 20px;
            margin-bottom: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5em;
            text-align: center;
            position: relative;
            overflow: hidden;
            animation: pulse 4s infinite;
        }

        .campaign-image::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: shimmer 3s infinite;
        }

        @keyframes shimmer {
            0% { transform: translateX(-100%) translateY(-100%); }
            100% { transform: translateX(100%) translateY(100%); }
        }

        .progress-section {
            background: var(--warm-gradient);
            padding: 25px;
            border-radius: 20px;
            margin: 30px 0;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .progress-bar {
            background: rgba(255, 255, 255, 0.3);
            height: 25px;
            border-radius: 15px;
            overflow: hidden;
            margin: 15px 0;
            box-shadow: inset 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .progress-fill {
            background: var(--success-gradient);
            height: 100%;
            width: 0%;
            transition: width 1s ease;
            border-radius: 15px;
            position: relative;
        }

        .progress-fill::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            animation: progressShine 2s infinite;
        }

        @keyframes progressShine {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }

        .progress-stats {
            display: flex;
            justify-content: space-between;
            margin-top: 15px;
            font-weight: 600;
        }

        .amount-raised {
            font-size: 2.2em;
            font-weight: 800;
            background: var(--success-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: pulse 2s infinite;
        }

        .donation-section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            position: sticky;
            top: 20px;
            animation: slideIn 1.4s ease;
        }

        .donation-title {
            background: var(--secondary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-size: 1.8em;
            font-weight: 700;
            margin-bottom: 25px;
            text-align: center;
        }

        .donation-amounts {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-bottom: 25px;
        }

        .amount-btn {
            padding: 20px;
            border: 3px solid transparent;
            background: var(--warm-gradient);
            border-radius: 15px;
            cursor: pointer;
            text-align: center;
            font-weight: 700;
            font-size: 1.1em;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .amount-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            transition: left 0.5s;
        }

        .amount-btn:hover::before {
            left: 100%;
        }

        .amount-btn:hover, .amount-btn.active {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            background: var(--primary-gradient);
            color: white;
        }

        .custom-amount {
            grid-column: 1 / -1;
            padding: 20px;
            border: 3px solid #e0e0e0;
            border-radius: 15px;
            font-size: 1.1em;
            text-align: center;
            margin-bottom: 25px;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .custom-amount:focus {
            outline: none;
            border-color: #ff6b9d;
            box-shadow: 0 0 20px rgba(255, 107, 157, 0.3);
        }

        .wallet-info {
            background: var(--warm-gradient);
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 25px;
            border-left: 5px solid #ff6b9d;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .wallet-address {
            font-family: 'Courier New', monospace;
            font-size: 0.85em;
            word-break: break-all;
            background: rgba(255, 255, 255, 0.8);
            padding: 15px;
            border-radius: 10px;
            margin-top: 15px;
            position: relative;
        }

        .donate-btn {
            width: 100%;
            padding: 20px;
            background: var(--primary-gradient);
            color: white;
            border: none;
            border-radius: 15px;
            font-size: 1.3em;
            font-weight: 800;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            animation: pulse 3s infinite;
        }

        .donate-btn::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.3), transparent);
            transform: rotate(45deg);
            transition: all 0.5s;
        }

        .donate-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(255, 107, 157, 0.4);
        }

        .donate-btn:hover::before {
            animation: shimmer 0.8s ease;
        }

        .copy-btn {
            background: var(--secondary-gradient);
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 0.85em;
            font-weight: 600;
            margin-left: 15px;
            transition: all 0.3s ease;
        }

        .copy-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .share-section {
            background: var(--warm-gradient);
            padding: 25px;
            border-radius: 20px;
            margin-top: 30px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .share-btn {
            display: inline-block;
            padding: 15px 25px;
            margin: 8px;
            background: var(--secondary-gradient);
            color: white;
            text-decoration: none;
            border-radius: 12px;
            font-weight: 600;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .share-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .recent-donations {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            animation: slideIn 1.6s ease;
        }

        .recent-donations h2 {
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-size: 2em;
            font-weight: 700;
            margin-bottom: 25px;
            text-align: center;
        }

        .donation-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            margin: 15px 0;
            background: var(--warm-gradient);
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .donation-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .donor-name {
            font-weight: 700;
            color: #333;
            font-size: 1.1em;
        }

        .donation-amount {
            background: var(--success-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-weight: 800;
            font-size: 1.2em;
        }

        .notification {
            position: fixed;
            top: 30px;
            right: 30px;
            background: var(--success-gradient);
            color: white;
            padding: 20px 25px;
            border-radius: 15px;
            display: none;
            z-index: 1000;
            font-weight: 600;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            animation: slideIn 0.5s ease;
        }

        .baby-emoji {
            font-size: 2em;
            animation: float 3s ease-in-out infinite;
            margin: 0 10px;
        }

        .heart-emoji {
            color: #ff6b9d;
            font-size: 1.5em;
            animation: pulse 1.5s infinite;
        }

        .story-highlight {
            background: var(--warm-gradient);
            padding: 25px;
            border-radius: 20px;
            margin: 20px 0;
            border-left: 5px solid #ff6b9d;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .milestone-card {
            background: var(--secondary-gradient);
            color: white;
            padding: 20px;
            border-radius: 15px;
            margin: 15px 0;
            text-align: center;
            font-weight: 600;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .milestone-card:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <div class="sparkles" id="sparkles"></div>
    
    <div class="notification" id="notification">✨ Address copied to clipboard!</div>
    
    <div class="container">
        <header>
            <div class="logo">👶 Help TJ Become a Super Dad! 💫</div>
            <div class="tagline">Supporting an amazing journey into fatherhood ✨</div>
        </header>

        <div class="main-content">
            <div class="campaign-section">
                <h1 class="campaign-title">Support TJ's Fatherhood Journey! <span class="baby-emoji">👶</span></h1>
                
                <div class="hero-section">
                    <h2 style="color: #333; margin-bottom: 15px; font-size: 1.5em;">🌟 A New Dad Needs Our Help! 🌟</h2>
                    <p style="font-size: 1.1em; color: #666; font-weight: 500;">
                        TJ is about to embark on the most incredible journey of his life - becoming a father! 
                        Let's come together to help him prepare for this beautiful adventure.
                    </p>
                </div>
                
                <div class="campaign-image">
                    <div>
                        👨‍👶 TJ's Fatherhood Journey<br>
                        <small style="opacity: 0.8;">Upload a beautiful family photo here! 📸</small>
                    </div>
                </div>

                <div class="progress-section">
                    <div class="amount-raised">$<span id="raised-amount">0</span> raised! <span class="heart-emoji">💖</span></div>
                    <div class="progress-bar">
                        <div class="progress-fill" id="progress-fill"></div>
                    </div>
                    <div class="progress-stats">
                        <span><strong>Goal: $<span id="goal-amount">15000</span></strong></span>
                        <span><strong><span id="donor-count">0</span> amazing supporters!</strong></span>
                    </div>
                </div>

                <div class="story-highlight">
                    <h3 style="color: #333; margin-bottom: 15px; font-size: 1.4em;">💝 Why TJ Needs Our Support</h3>
                    <p style="margin-bottom: 15px;">
                        <strong>TJ is preparing to become a first-time dad!</strong> 🎉 This life-changing moment comes with incredible joy but also significant expenses and preparations. From baby essentials to setting up the perfect nursery, every dollar helps TJ create the best possible start for his little one.
                    </p>
                    
                    <p style="margin-bottom: 15px;">
                        As someone who's always been there for others, TJ now needs our community to rally around him during this special time. Your contribution isn't just money - it's love, support, and belief in TJ's journey as a new parent.
                    </p>

                    <div style="text-align: center; margin: 20px 0;">
                        <span style="font-size: 2em;">👶💕👨‍👩‍👧‍👦💕🍼</span>
                    </div>
                </div>

                <div class="milestone-card">
                    <h3 style="margin-bottom: 10px;">🎯 How Your Donation Helps:</h3>
                    <p><strong>• Baby Essentials:</strong> Diapers, formula, clothes, and more!</p>
                    <p><strong>• Nursery Setup:</strong> Crib, changing table, decorations</p>
                    <p><strong>• Medical Expenses:</strong> Doctor visits and healthcare</p>
                    <p><strong>• Emergency Fund:</strong> Peace of mind for unexpected needs</p>
                    <p><strong>• Parent Prep:</strong> Books, classes, and resources</p>
                </div>

                <div class="story-highlight">
                    <h3 style="color: #333; margin-bottom: 15px;">✨ Join TJ's Village!</h3>
                    <p>
                        They say it takes a village to raise a child - and we want YOU to be part of TJ's village! 
                        Every contribution, no matter the size, shows TJ that he's not alone in this incredible journey. 
                        Together, we can help him become the amazing father we know he'll be! <span class="heart-emoji">💖</span>
                    </p>
                </div>

                <div class="share-section">
                    <h3 style="margin-bottom: 20px; color: #333;">🚀 Spread the Love!</h3>
                    <a href="#" class="share-btn" onclick="shareOnTwitter()">📱 Twitter</a>
                    <a href="#" class="share-btn" onclick="shareOnFacebook()">📘 Facebook</a>
                    <a href="#" class="share-btn" onclick="shareOnInstagram()">📸 Instagram</a>
                    <a href="#" class="share-btn" onclick="copyLink()">🔗 Copy Link</a>
                </div>
            </div>

            <div class="donation-section">
                <h2 class="donation-title">💝 Donate to TJ's Dad Fund!</h2>
                
                <div style="text-align: center; margin-bottom: 20px; font-size: 1.1em; color: #666;">
                    <span class="baby-emoji">👶</span> Help create magic for a new family! <span class="baby-emoji">✨</span>
                </div>
                
                <div class="donation-amounts">
                    <div class="amount-btn" onclick="selectAmount(50)">💫 $50<br><small>Baby Basics</small></div>
                    <div class="amount-btn" onclick="selectAmount(100)">🌟 $100<br><small>Nursery Love</small></div>
                    <div class="amount-btn" onclick="selectAmount(250)">💖 $250<br><small>Dad Supporter</small></div>
                    <div class="amount-btn" onclick="selectAmount(500)">🎉 $500<br><small>Super Hero</small></div>
                </div>

                <input type="number" class="custom-amount" id="custom-amount" placeholder="💰 Enter your special amount ($)" min="1">

                <div class="wallet-info">
                    <strong style="color: #333;">🔐 Solana Wallet Address:</strong>
                    <div class="wallet-address">
                        2ZruidkAbYoH63dCSMYkcYsSugc3fQW2s3TftKi4eE5S
                        <button class="copy-btn" onclick="copyWalletAddress()">📋 Copy</button>
                    </div>
                    <small style="color: #666; margin-top: 10px; display: block;">
                        ⚡ Send SOL directly to this address - fast, secure, and blockchain-powered!
                    </small>
                </div>

                <button class="donate-btn" onclick="processDonation()">
                    🚀 DONATE NOW & HELP TJ! ✨
                </button>

                <div style="margin-top: 20px; text-align: center; font-size: 0.95em; color: #666;">
                    <p><span class="heart-emoji">💖</span> <strong>100% Secure Blockchain Magic</strong></p>
                    <p>⚡ <strong>Instant Direct Transfer to TJ</strong></p>
                    <p>🌟 <strong>Be Part of Something Beautiful</strong></p>
                </div>
            </div>
        </div>

        <div class="recent-donations">
            <h2>🌟 Amazing Supporters! 🌟</h2>
            <div id="donations-list">
                <div class="donation-item">
                    <div>
                        <div class="donor-name">Sarah & Mike 💕</div>
                        <div style="color: #666; font-size: 0.9em;">2 hours ago • "So excited for you TJ!"</div>
                    </div>
                    <div class="donation-amount">$100.00</div>
                </div>
                <div class="donation-item">
                    <div>
                        <div class="donor-name">Anonymous Angel 👼</div>
                        <div style="color: #666; font-size: 0.9em;">5 hours ago • "You'll be an amazing dad!"</div>
                    </div>
                    <div class="donation-amount">$75.00</div>
                </div>
                <div class="donation-item">
                    <div>
                        <div class="donor-name">The Johnson Family 👨‍👩‍👧‍👦</div>
                        <div style="color: #666; font-size: 0.9em;">1 day ago • "Welcome to parenthood!"</div>
                    </div>
                    <div class="donation-amount">$200.00</div>
                </div>
                <div class="donation-item">
                    <div>
                        <div class="donor-name">Best Friend Lisa 👯‍♀️</div>
                        <div style="color: #666; font-size: 0.9em;">2 days ago • "Can't wait to meet the little one!"</div>
                    </div>
                    <div class="donation-amount">$150.00</div>
                </div>
            </div>
        </div>
    </div>

    <script>
        const WALLET_ADDRESS = "2ZruidkAbYoH63dCSMYkcYsSugc3fQW2s3TftKi4eE5S";
        let selectedAmount = 0;
        let totalRaised = 525; // Starting amount from sample donations
        let donorCount = 4;
        let goalAmount = 15000;

        // Create sparkles animation
        function createSparkles() {
            const sparklesContainer = document.getElementById('sparkles');
            for (let i = 0; i < 20; i++) {
                const sparkle = document.createElement('div');
                sparkle.className = 'sparkle';
                sparkle.style.left = Math.random() * 100 + '%';
                sparkle.style.top = Math.random() * 100 + '%';
                sparkle.style.animationDelay = Math.random() * 3 + 's';
                sparklesContainer.appendChild(sparkle);
            }
        }

        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            createSparkles();
            updateProgress();
            
            // Add some dynamic effects
            setTimeout(() => {
                document.querySelector('.donate-btn').style.animation = 'pulse 2s infinite, float 4s ease-in-out infinite';
            }, 2000);
        });

        function selectAmount(amount) {
            selectedAmount = amount;
            document.getElementById('custom-amount').value = amount;
            
            // Update button states with animation
            document.querySelectorAll('.amount-btn').forEach(btn => {
                btn.classList.remove('active');
                btn.style.transform = 'scale(1)';
            });
            
            event.target.classList.add('active');
            event.target.style.transform = 'scale(1.1)';
            
            // Add celebratory effect
            createCelebrationEffect(event.target);
        }

        function createCelebrationEffect(element) {
            const rect = element.getBoundingClientRect();
            for (let i = 0; i < 5; i++) {
                const heart = document.createElement('div');
                heart.innerHTML = '💖';
                heart.style.position = 'fixed';
                heart.style.left = rect.left + rect.width/2 + 'px';
                heart.style.top = rect.top + rect.height/2 + 'px';
                heart.style.fontSize = '20px';
                heart.style.pointerEvents = 'none';
                heart.style.zIndex = '1000';
                heart.style.animation = `floatUp 2s ease-out forwards`;
                heart.style.transform = `translateX(${(Math.random() - 0.5) * 100}px)`;
                document.body.appendChild(heart);
                
                setTimeout(() => {
                    document.body.removeChild(heart);
                }, 2000);
            }
        }

        // Add float up animation for hearts
        const style = document.createElement('style');
        style.textContent = `
            @keyframes floatUp {
                0% { transform: translateY(0) scale(1); opacity: 1; }
                100% { transform: translateY(-100px) scale(0.5); opacity: 0; }
            }
        `;
        document.head.appendChild(style);

        function updateProgress() {
            const percentage = Math.min((totalRaised / goalAmount) * 100, 100);
            const progressFill = document.getElementById('progress-fill');
            
            // Animate progress bar
            setTimeout(() => {
                progressFill.style.width = percentage + '%';
            }, 500);
            
            // Animate numbers
            animateNumber('raised-amount', totalRaised, 2000);
            animateNumber('donor-count', donorCount, 1500);
            document.getElementById('goal-amount').textContent = goalAmount.toLocaleString();
            
            // Add celebration if goal is reached
            if (percentage >= 100) {
                celebrateGoalReached();
            }
        }

        function animateNumber(elementId, targetValue, duration) {
            const element = document.getElementById(elementId);
            const startValue = parseInt(element.textContent) || 0;
            const increment = (targetValue - startValue) / (duration / 50);
            let currentValue = startValue;
            
            const timer = setInterval(() => {
                currentValue += increment;
                if ((increment > 0 && currentValue >= targetValue) || 
                    (increment < 0 && currentValue <= targetValue)) {
                    currentValue = targetValue;
                    clearInterval(timer);
                }
                element.textContent = Math.floor(currentValue).toLocaleString();
            }, 50);
        }

        function celebrateGoalReached() {
            // Create celebration effect
            for (let i = 0; i < 30; i++) {
                setTimeout(() => {
                    createFloatingEmoji(['🎉', '🥳', '👶', '💖', '✨'][Math.floor(Math.random() * 5)]);
                }, i * 100);
            }
            
            // Show special message
            setTimeout(() => {
                alert('🎉 AMAZING! We reached our goal! TJ is going to be so grateful! 👶💖');
            }, 2000);
        }

        function createFloatingEmoji(emoji) {
            const element = document.createElement('div');
            element.innerHTML = emoji;
            element.style.position = 'fixed';
            element.style.left = Math.random() * window.innerWidth + 'px';
            element.style.top = window.innerHeight + 'px';
            element.style.fontSize = '30px';
            element.style.pointerEvents = 'none';
            element.style.zIndex = '1000';
            element.style.animation = 'floatUp 3s ease-out forwards';
            document.body.appendChild(element);
            
            setTimeout(() => {
                document.body.removeChild(element);
            }, 3000);
        }

        function copyWalletAddress() {
            navigator.clipboard.writeText(WALLET_ADDRESS).then(function() {
                showNotification('✨ Wallet address copied! Ready to make magic happen! 🚀');
                createCelebrationBurst();
            }).catch(function(err) {
                console.error('Could not copy text: ', err);
                // Fallback for older browsers
                const textArea = document.createElement('textarea');
                textArea.value = WALLET_ADDRESS;
                document.body.appendChild(textArea);
                textArea.select();
                document.execCommand('copy');
                document.body.removeChild(textArea);
                showNotification('✨ Wallet address copied! Ready to make magic happen! 🚀');
                createCelebrationBurst();
            });
        }

        function createCelebrationBurst() {
            const emojis = ['✨', '💫', '⭐', '🌟', '💖'];
            for (let i = 0; i < 10; i++) {
                setTimeout(() => {
                    createFloatingEmoji(emojis[Math.floor(Math.random() * emojis.length)]);
                }, i * 50);
            }
        }

        function processDonation() {
            const customAmount = document.getElementById('custom-amount').value;
            const donationAmount = customAmount || selectedAmount;

            if (!donationAmount || donationAmount <= 0) {
                showNotification('💫 Please select or enter a donation amount to help TJ! 👶', 'warning');
                return;
            }

            // Create custom celebration message
            const messages = [
                `🎉 You're about to make TJ's day with $${donationAmount}!`,
                `👶 This $${donationAmount} will help TJ become an amazing dad!`,
                `💖 Your $${donationAmount} donation is pure love for TJ's family!`,
                `✨ $${donationAmount} of pure kindness heading TJ's way!`
            ];
            
            const randomMessage = messages[Math.floor(Math.random() * messages.length)];

            // Enhanced donation instructions with celebration
            alert(`${randomMessage}\n\n🚀 TO COMPLETE YOUR DONATION:\n\n1. 📋 Copy wallet address: ${WALLET_ADDRESS}\n2. 💜 Open your Solana wallet app\n3. 💫 Send $${donationAmount} worth of SOL\n4. ✨ Watch the magic happen!\n\n👶 TJ and his future little one thank you from the bottom of their hearts! 💖\n\nYou're helping create something beautiful! 🌟`);

            // Simulate the donation with celebration
            simulateDonation(donationAmount);
            createMegaCelebration();
        }

        function createMegaCelebration() {
            // Big celebration effect
            const celebrationEmojis = ['🎉', '🥳', '👶', '💖', '✨', '🌟', '💫', '🎊'];
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    createFloatingEmoji(celebrationEmojis[Math.floor(Math.random() * celebrationEmojis.length)]);
                }, i * 100);
            }
            
            // Flash effect
            document.body.style.background = 'linear-gradient(45deg, #ff9a9e, #fad0c4, #ffd1ff, #ff9a9e)';
            setTimeout(() => {
                document.body.style.background = 'linear-gradient(45deg, #ff9a9e, #fecfef, #fecfef, #ff9a9e)';
            }, 500);
        }

        function simulateDonation(amount) {
            totalRaised += parseFloat(amount);
            donorCount += 1;
            updateProgress();

            // Add to recent donations with celebration
            addRecentDonation('You (Just now!) 🌟', amount, 'Thank you for being amazing! 💖');
            
            // Show success message
            setTimeout(() => {
                showNotification(`🎉 Your $${amount} donation is processing! TJ will be so grateful! 👶💖`, 'success');
            }, 1000);
        }

        function addRecentDonation(donor, amount, message = '') {
            const donationsList = document.getElementById('donations-list');
            const donationItem = document.createElement('div');
            donationItem.className = 'donation-item';
            donationItem.style.animation = 'slideIn 0.8s ease, pulse 2s infinite';
            donationItem.innerHTML = `
                <div>
                    <div class="donor-name">${donor}</div>
                    <div style="color: #666; font-size: 0.9em;">Just now • "${message}"</div>
                </div>
                <div class="donation-amount">$${parseFloat(amount).toFixed(2)}</div>
            `;
            donationsList.insertBefore(donationItem, donationsList.firstChild);
            
            // Remove animation after a while
            setTimeout(() => {
                donationItem.style.animation = 'none';
            }, 4000);
        }

        function showNotification(message, type = 'success') {
            const notification = document.getElementById('notification');
            notification.innerHTML = message;
            notification.style.display = 'block';
            
            if (type === 'warning') {
                notification.style.background = 'linear-gradient(135deg, #ff6b9d, #f8b500)';
            } else {
                notification.style.background = 'linear-gradient(135deg, #4facfe, #00f2fe)';
            }
            
            setTimeout(() => {
                notification.style.display = 'none';
            }, 4000);
        }

        function shareOnTwitter() {
            const text = encodeURIComponent("🎉 Help TJ become an amazing dad! 👶✨ Every donation helps create something beautiful for a new family! 💖 #DadSupport #NewDad #Community");
            const url = encodeURIComponent(window.location.href);
            window.open(`https://twitter.com/intent/tweet?text=${text}&url=${url}`, '_blank');
            createCelebrationBurst();
        }

        function shareOnFacebook() {
            const url = encodeURIComponent(window.location.href);
            window.open(`https://www.facebook.com/sharer/sharer.php?u=${url}`, '_blank');
            createCelebrationBurst();
        }

        function shareOnInstagram() {
            showNotification('📸 Copy the link and share TJ\'s story on Instagram! Every share helps! ✨');
            copyLink();
        }

        function copyLink() {
            navigator.clipboard.writeText(window.location.href).then(function() {
                showNotification('🔗 Campaign link copied! Share TJ\'s story everywhere! 🚀✨');
                createCelebrationBurst();
            });
        }

        // Handle custom amount input with celebration
        document.getElementById('custom-amount').addEventListener('input', function() {
            selectedAmount = 0;
            document.querySelectorAll('.amount-btn').forEach(btn => {
                btn.classList.remove('active');
                btn.style.transform = 'scale(1)';
            });
            
            // Add sparkle effect to input
            if (this.value > 0) {
                this.style.borderColor = '#ff6b9d';
                this.style.boxShadow = '0 0 20px rgba(255, 107, 157, 0.3)';
            }
        });

        // Add hover effects to donation buttons
        document.querySelectorAll('.amount-btn').forEach(btn => {
            btn.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-2px) scale(1.02)';
            });
            
            btn.addEventListener('mouseleave', function() {
                if (!this.classList.contains('active')) {
                    this.style.transform = 'scale(1)';
                }
            });
        });

        // Add periodic sparkle effects
        setInterval(() => {
            if (Math.random() > 0.7) {
                createFloatingEmoji(['✨', '💫', '⭐'][Math.floor(Math.random() * 3)]);
            }
        }, 3000);

        // Welcome message
        setTimeout(() => {
            showNotification('👶 Welcome to TJ\'s Dad Fund! Every donation creates magic! ✨', 'success');
        }, 2000);
    </script>
</body>
</html>
