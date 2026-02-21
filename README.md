<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🧱 concrete · human guide</title>
    <!-- Font & Icons -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300..700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            background: #f4f1eb;  /* warm paper background */
            color: #1a2a33;
            line-height: 1.5;
            padding: 20px;
            min-height: 100vh;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
        }
        /* glassy, soft card */
        .card {
            background: rgba(255, 255, 255, 0.75);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-radius: 40px;
            padding: 32px 28px;
            box-shadow: 0 25px 50px -12px rgba(0, 30, 40, 0.25),
                        0 2px 10px 0 rgba(255, 255, 240, 0.6) inset;
            border: 1px solid rgba(255, 245, 235, 0.6);
        }
        .welcome-block {
            background: linear-gradient(155deg, #ffe6d5 0%, #fff2e0 100%);
            border-radius: 40px;
            padding: 32px 28px;
            margin-bottom: 24px;
            box-shadow: 0 15px 30px -12px #b29e88;
            border: 1px solid #ffefdb;
        }
        h1 {
            font-size: 2.2rem;
            font-weight: 600;
            letter-spacing: -0.02em;
            color: #1f3b4a;
            margin-bottom: 16px;
        }
        h1 span {
            background: #1f3b4a;
            color: #ffe6d0;
            padding: 4px 14px;
            border-radius: 60px;
            font-size: 1.3rem;
            display: inline-block;
            margin-top: 8px;
        }
        .greeting {
            font-size: 1.2rem;
            margin: 20px 0;
            padding: 0 0 0 22px;
            border-left: 5px solid #c5785e;
            font-weight: 400;
            color: #2d4a5a;
        }
        .pill-stats {
            display: flex;
            flex-wrap: wrap;
            gap: 14px;
            margin: 24px 0 8px;
        }
        .pill {
            background: rgba(31, 59, 74, 0.85);
            backdrop-filter: blur(4px);
            color: #f0e7db;
            padding: 8px 22px;
            border-radius: 60px;
            font-size: 0.95rem;
            font-weight: 500;
            box-shadow: 0 6px 14px rgba(0,0,0,0.1);
            border: 1px solid rgba(255,255,220,0.3);
        }
        .button-grid {
            display: flex;
            flex-direction: column;
            gap: 14px;
            margin: 28px 0 20px;
        }
        .guide-btn {
            background: white;
            border: none;
            border-radius: 120px;
            padding: 18px 26px;
            font-size: 1.25rem;
            font-weight: 500;
            text-align: left;
            display: flex;
            align-items: center;
            gap: 20px;
            width: 100%;
            box-shadow: 0 6px 16px rgba(0,0,0,0.03);
            transition: all 0.2s ease;
            border: 1px solid #f0e2d4;
            cursor: pointer;
            color: #1f3b4a;
        }
        .guide-btn:hover {
            transform: translateY(-4px);
            box-shadow: 0 25px 35px -12px #b2a088;
            border-color: #c9ad93;
            background: #fffaf5;
        }
        .guide-btn .emoji {
            font-size: 2.2rem;
            min-width: 56px;
            filter: drop-shadow(2px 4px 6px rgba(0,0,0,0.1));
        }
        .arrow-hint {
            margin-left: auto;
            font-size: 1.8rem;
            color: #b6a089;
            transition: 0.2s;
        }
        .guide-btn:hover .arrow-hint {
            transform: translateX(4px);
            color: #7d5f4b;
        }
        /* detail panel */
        .detail-panel {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(16px);
            border-radius: 36px;
            padding: 30px 30px 36px;
            margin: 20px 0 30px;
            box-shadow: 0 30px 50px -20px #a48e7a;
            border: 1px solid rgba(255, 235, 215, 0.7);
        }
        .detail-content {
            font-size: 1.05rem;
            color: #1a333f;
        }
        .detail-content h3 {
            font-size: 1.9rem;
            font-weight: 600;
            margin-bottom: 24px;
            color: #1f3b4a;
            letter-spacing: -0.01em;
            display: flex;
            align-items: center;
            gap: 12px;
            border-bottom: 3px solid #ffb08a;
            padding-bottom: 12px;
        }
        .detail-content p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            line-height: 1.6;
        }
        .detail-content ul, .detail-content ol {
            margin: 18px 0 22px;
            padding-left: 28px;
        }
        .detail-content li {
            margin-bottom: 14px;
            font-size: 1.05rem;
            list-style-type: '✨ ';
        }
        .detail-content li::marker {
            color: #c96e4b;
            font-size: 1.2rem;
        }
        .insight-box {
            background: #fae9de;
            border-radius: 28px;
            padding: 22px 26px;
            margin: 30px 0 20px;
            border-left: 8px solid #bf7f60;
            font-weight: 400;
            box-shadow: inset 0 2px 8px #ffe7d6;
        }
        .link-list {
            display: flex;
            flex-wrap: wrap;
            gap: 16px;
            margin: 25px 0 5px;
        }
        .link-list a {
            background: #1f3b4a;
            color: white;
            padding: 12px 26px;
            border-radius: 60px;
            text-decoration: none;
            font-weight: 500;
            transition: 0.2s;
            border: 1px solid #ffffff50;
        }
        .link-list a:hover {
            background: #152d39;
            transform: scale(1.02);
            box-shadow: 0 12px 20px -12px #1f3b4a;
        }
        .human-note {
            margin-top: 35px;
            background: #f5e7dc;
            border-radius: 32px;
            padding: 20px 28px;
            text-align: center;
            font-size: 1rem;
            color: #4d3629;
            border: 2px dashed #dbb59b;
        }
        .footer {
            margin-top: 40px;
            text-align: center;
            color: #6f5e4e;
            font-size: 0.95rem;
        }
        hr {
            border: 1px solid #ddc7b6;
            margin: 28px 0;
        }
    </style>
</head>
<body>
<div class="container">
    <!-- WELCOME – warm, human -->
    <div class="welcome-block">
        <h1>hey there 👋 <br><span>welcome to concrete land</span></h1>
        <div class="greeting">
            Concrete isn’t some hype machine — it’s real infrastructure for people who care about capital efficiency. I’ve packed everything I know into this little guide. hope it helps you find your way 🧱
        </div>
        <div class="pill-stats">
            <span class="pill">🗿 moai wisdom</span>
            <span class="pill">🔑 acces role</span>
            <span class="pill">🏆 badge levels 5–25</span>
            <span class="pill">📝 article 101</span>
        </div>
    </div>

    <!-- BUTTON grid (dynamically filled) -->
    <div id="buttonContainer" class="button-grid"></div>

    <!-- DETAIL panel shows after click -->
    <div id="detailPanel" class="detail-panel">
        <div class="detail-content" id="detailContent">
            <h3>🧱 tap any button above 👆</h3>
            <p style="font-size: 1.2rem;">I’ve written down step‑by‑step what I’ve learned about Concrete — from vaults to moai. no fluff, just real talk.</p>
            <div class="insight-box">
                💬 a quick human thought: this place is built by people like you and me. the more we share what we know, the stronger it gets.
            </div>
        </div>
    </div>

    <!-- quick official links + ecosystem -->
    <div class="human-note">
        <div style="display: flex; gap: 12px; flex-wrap: wrap; justify-content: center; margin-bottom: 12px;">
            <a href="https://concrete.xyz" target="_blank" style="color:#1f3b4a; font-weight:600;">🏠 concrete.xyz</a>
            <a href="https://docs.concrete.xyz" target="_blank" style="color:#1f3b4a;">📘 docs</a>
            <a href="https://points.concrete.xyz" target="_blank" style="color:#1f3b4a;">⭐ points</a>
            <a href="https://concrete.xyz/ecosystem" target="_blank" style="color:#1f3b4a;">🌿 ecosystem</a>
        </div>
        <div>💡 these are the real places — always double‑check, but they’re safe.</div>
    </div>

    <div class="footer">
        written by a community learner, for new friends. ✨ last updated feb 2026
    </div>
</div>

<script>
    // All the content — rewritten in a natural, human tone (no bullet symbols, just friendly)
    const sections = [
        {
            id: 'what',
            emoji: '🧱',
            label: 'what is concrete?',
            content: `
                <h3>🧱 what is concrete?</h3>
                <p>Concrete is DeFi infrastructure — not some quick farm. It’s built for real capital efficiency, automated strategies, and long term thinking. no hype, just solid rails.</p>
                <p>they focus on:</p>
                <ul><li>automated vaults that work like smart portfolios</li><li>reducing idle capital and compounding for you</li><li>institutional style but onchain and open</li></ul>
                <p>official home: <a href="https://concrete.xyz" target="_blank">concrete.xyz</a> — docs are really good too: <a href="https://docs.concrete.xyz/Overview/welcome/" target="_blank">welcome page</a></p>
            `
        },
        {
            id: 'vaults',
            emoji: '💰',
            label: 'concrete vaults',
            content: `
                <h3>💰 vaults — your automated money manager</h3>
                <p>vaults are like having a robot that puts your crypto to work. they:</p>
                <ul><li>move funds across strategies so nothing sits idle</li><li>auto‑compound returns without you lifting a finger</li><li>use standards like ERC‑4626, so they play nice with other defi tools</li></ul>
                <p>they’re not just “deposit and hope”. they’re more like programmable finance. read more in the <a href="https://concrete.xyz/blog-articles-list/concrete-vaults-participate-in-defi-without-becoming-a-defi-expert" target="_blank">vault blog post</a>.</p>
            `
        },
        {
            id: 'app',
            emoji: '🌐',
            label: 'the concrete app',
            content: `
                <h3>🌐 app — where you see everything</h3>
                <p>the app is your dashboard. you can:</p>
                <ul><li>see your vault positions and performance</li><li>track how efficiently your capital is used</li><li>enter new strategies and manage allocations</li></ul>
                <p>just go to <a href="https://concrete.xyz" target="_blank">concrete.xyz</a> and hit “launch app”. super clean.</p>
            `
        },
        {
            id: 'points',
            emoji: '⭐',
            label: 'points & referral',
            content: `
                <h3>⭐ points and inviting friends</h3>
                <p>concrete runs a points system where you earn by doing stuff — writing articles, helping on discord, or joining campaigns. check your progress at <a href="https://points.concrete.xyz/profile" target="_blank">points.concrete.xyz</a>.</p>
                <p>referral programs pop up sometimes: you share a link, people join, you get recognised. always check the official announcements in discord for current rewards.</p>
                <div class="insight-box">💡 tip: share your referral in #referrals channel, but don’t spam — be part of the convo.</div>
            `
        },
        {
            id: 'badges',
            emoji: '🏆',
            label: 'badge levels (5,10,17,25...)',
            content: `
                <h3>🏆 badges show your vibe</h3>
                <p>badges are like little milestones that grow as you contribute. they reflect:</p>
                <ul><li>being around consistently</li><li>having good conversations</li><li>helping others figure things out</li><li>sharing content or ideas</li></ul>
                <p>levels like 5, 10, 17, 25 — each one means you’re more part of the fabric. there’s no cheat sheet, just genuine involvement.</p>
            `
        },
        {
            id: 'access',
            emoji: '🔑',
            label: 'the acces role',
            content: `
                <h3>🔑 acces — for people who truly give</h3>
                <p>acces is given to those who’ve put in meaningful effort. things like:</p>
                <ul><li>helping newbies with patience</li><li>writing thoughtful content</li><li>being a positive presence in discord</li></ul>
                <p>how it works: current acces holders nominate someone they think deserves it. if the team agrees, that person gets the 🔑. so it’s not about asking — it’s about being so helpful that others notice.</p>
            `
        },
        {
            id: 'moai',
            emoji: '🗿',
            label: 'moai role (hand‑picked)',
            content: `
                <h3>🗿 moai — the most dedicated</h3>
                <p>moai are chosen directly by the team. they’re the ones who:</p>
                <ul><li>guide and support others every day</li><li>create solid content on X (twitter) that spreads the word</li><li>show up consistently, not just when something’s trending</li></ul>
                <div class="insight-box">my own take: don’t chase it. just share what you’re good at, put in the work, and let your efforts speak. consistency + genuine care is the way.</div>
            `
        },
        {
            id: 'article',
            emoji: '✍️',
            label: 'writing articles (easy mode)',
            content: `
                <h3>✍️ how to write and submit articles</h3>
                <p>if you’ve got X premium, you can post threads there and drop the link. but if you don’t, Medium is super simple:</p>
                <ol><li>grab the Medium app from Play Store</li><li>tap the pencil icon and start writing — keep it real, not like an essay</li><li>hit preview, then publish</li><li>go to your profile, tap the three dots on your article, and copy the link</li><li>paste it on the Concrete points site or share in discord #content</li></ol>
                <p>pro tip: write about what helped you — vaults, roles, or just why you like the project. simple is good.</p>
            `
        },
        {
            id: 'ecosystem',
            emoji: '🤝',
            label: 'ecosystem & backup',
            content: `
                <h3>🤝 who’s building with concrete</h3>
                <p>concrete works with other solid protocols like Pendle, Morpho, and more. you can see the full list on their <a href="https://concrete.xyz/ecosystem" target="_blank">ecosystem page</a>.</p>
                <p>the whole idea is to be infrastructure, not just another app. that’s why they focus on long‑term partnerships and real use.</p>
            `
        }
    ];

    const buttonContainer = document.getElementById('buttonContainer');
    const detailPanel = document.getElementById('detailPanel');
    const detailContent = document.getElementById('detailContent');

    // render all buttons
    function renderButtons() {
        let html = '';
        sections.forEach(s => {
            html += `<button class="guide-btn" data-id="${s.id}">
                <span class="emoji">${s.emoji}</span>
                <span>${s.label}</span>
                <span class="arrow-hint">↝</span>
            </button>`;
        });
        buttonContainer.innerHTML = html;

        // attach click
        document.querySelectorAll('.guide-btn').forEach(btn => {
            btn.addEventListener('click', (e) => {
                const id = btn.dataset.id;
                const section = sections.find(s => s.id === id);
                if (section) {
                    detailContent.innerHTML = section.content;
                    // smooth scroll to detail
                    detailPanel.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    }

    renderButtons();
</script>
</body>
</html>
