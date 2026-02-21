<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🧱 Concrete Guide • Newbie Welcome</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Segoe UI', Roboto, system-ui, sans-serif;
            background: #f4f7fb;
            color: #1a2639;
            padding: 20px;
            min-height: 100vh;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
        }
        /* welcome card */
        .welcome-card {
            background: linear-gradient(145deg, #0b1e33 0%, #1a3650 100%);
            color: white;
            padding: 30px 25px;
            border-radius: 32px;
            margin-bottom: 24px;
            box-shadow: 0 20px 30px -10px rgba(0,20,40,0.3);
        }
        .welcome-card h1 {
            font-size: 2.2rem;
            line-height: 1.2;
            margin-bottom: 15px;
            font-weight: 600;
        }
        .welcome-card h1 span {
            background: #ffd966;
            color: #0b1e33;
            padding: 4px 12px;
            border-radius: 40px;
            font-size: 1.2rem;
            display: inline-block;
            margin-top: 8px;
        }
        .welcome-message {
            font-size: 1.1rem;
            opacity: 0.95;
            margin-bottom: 20px;
            border-left: 4px solid #ffd966;
            padding-left: 18px;
        }
        .stats-mini {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            font-size: 0.9rem;
            background: rgba(255,255,255,0.1);
            padding: 15px;
            border-radius: 24px;
            backdrop-filter: blur(4px);
        }
        /* main grid */
        .button-grid {
            display: flex;
            flex-direction: column;
            gap: 12px;
            margin-bottom: 30px;
        }
        .guide-btn {
            background: white;
            border: none;
            border-radius: 28px;
            padding: 18px 24px;
            font-size: 1.2rem;
            font-weight: 600;
            text-align: left;
            display: flex;
            align-items: center;
            gap: 16px;
            box-shadow: 0 6px 14px rgba(0,0,0,0.04);
            cursor: pointer;
            transition: 0.2s ease;
            border: 1px solid rgba(0,0,0,0.02);
            color: #1a2b3c;
            width: 100%;
        }
        .guide-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 15px 25px -8px rgba(0,60,120,0.2);
            border-color: #b0c9e8;
        }
        .guide-btn .emoji-big {
            font-size: 2rem;
            min-width: 48px;
        }
        .arrow {
            margin-left: auto;
            font-size: 1.5rem;
            color: #7c8b9c;
        }
        /* expandable detail panel */
        .detail-panel {
            background: white;
            border-radius: 28px;
            padding: 0;
            margin-top: -8px;
            margin-bottom: 8px;
            box-shadow: 0 12px 28px rgba(0,0,0,0.03);
            border: 1px solid #e2eaf2;
            overflow: hidden;
            transition: all 0.2s;
        }
        .detail-content {
            padding: 22px 28px 28px 28px;
            background: #ffffff;
        }
        .detail-content h3 {
            font-size: 1.5rem;
            margin-bottom: 16px;
            color: #11324b;
            border-bottom: 2px solid #ffd966;
            padding-bottom: 6px;
            display: inline-block;
        }
        .detail-content p, .detail-content li {
            font-size: 1rem;
            line-height: 1.6;
            color: #253c5c;
            margin-bottom: 12px;
        }
        .detail-content ul, .detail-content ol {
            padding-left: 24px;
            margin: 16px 0;
        }
        .detail-content li {
            margin-bottom: 8px;
        }
        .badge {
            background: #f0f6ff;
            border-radius: 30px;
            padding: 14px 20px;
            margin: 18px 0 8px;
            border-left: 5px solid #2b6c9e;
            font-weight: 500;
        }
        .code-note {
            background: #0e1e2f;
            color: #d4e6ff;
            padding: 14px 18px;
            border-radius: 20px;
            font-family: monospace;
            font-size: 0.95rem;
            margin: 20px 0 0;
            white-space: pre-wrap;
        }
        .button-link {
            background: #1a3a57;
            color: white;
            border: none;
            border-radius: 40px;
            padding: 12px 24px;
            font-weight: 600;
            font-size: 1rem;
            cursor: pointer;
            margin: 8px 6px 0 0;
            display: inline-block;
            text-decoration: none;
        }
        .button-link:hover {
            background: #11324b;
        }
        .footer {
            text-align: center;
            margin: 42px 0 20px;
            color: #5c6f87;
            font-size: 0.95rem;
        }
        hr {
            border: 1px solid #d3e0ec;
            margin: 24px 0;
        }
        .hidden {
            display: none;
        }
        .official-links {
            background: #ecf3fa;
            border-radius: 24px;
            padding: 16px 22px;
            margin-top: 25px;
        }
    </style>
</head>
<body>
<div class="container">
    <!-- WELCOME CARD (human, warm) -->
    <div class="welcome-card">
        <h1>👋 welcome to <span>concrete</span><br>your starter pack 🧱</h1>
        <div class="welcome-message">
            Concrete isn't just another defi project — it's infrastructure for real capital efficiency.<br>
            This guide is built by a community member, for newbies. no hype, just steps.
        </div>
        <div class="stats-mini">
            <span>🗿 moai guide</span>
            <span>🔑 acces role</span>
            <span>🏆 badge levels 5–25</span>
            <span>📝 article 101</span>
        </div>
    </div>

    <!-- BUTTONS (each opens a detail) -->
    <div class="button-grid" id="buttonGrid">
        <!-- will be populated by JS but we can write static then dynamic -->
    </div>
    <!-- detail container -->
    <div id="detailContainer"></div>

    <!-- quick links / footer -->
    <div class="official-links">
        <div style="display: flex; gap: 16px; flex-wrap: wrap; align-items: center;">
            <span style="font-weight: 600;">🔗 official:</span>
            <a href="https://concrete.xyz" target="_blank" style="color: #1d4d7c;">concrete.xyz</a>
            <a href="https://docs.concrete.xyz" target="_blank" style="color: #1d4d7c;">docs</a>
            <a href="https://points.concrete.xyz" target="_blank" style="color: #1d4d7c;">points</a>
            <a href="https://concrete.xyz/ecosystem" target="_blank" style="color: #1d4d7c;">ecosystem</a>
        </div>
        <div style="margin-top: 12px; font-style: italic; color: #3d5a78;">
            💡 tip: bookmark this — i update when community info evolves
        </div>
    </div>

    <div class="footer">
        ⛓️ built with 🧱 for concrete community • human made • not official, just helpful
    </div>
</div>

<script>
    // ---------- all content you provided, organised ----------
    const sections = [
        {
            id: 'what',
            emoji: '🧱',
            label: 'What is Concrete?',
            content: `
                <h3>🏗️ what is concrete?</h3>
                <p><strong>Concrete is DeFi infrastructure, not a short‑term farm.</strong> It focuses on capital‑efficiency and automated, institutional‑style onchain finance — not chasing APY hype.</p>
                <p>Core philosophy: <em>“backbone of DeFi finance, not just yield products.”</em></p>
                <p>🔗 official: <a href="https://concrete.xyz" target="_blank">concrete.xyz</a> · <a href="https://docs.concrete.xyz/Overview/welcome/" target="_blank">welcome docs</a></p>
            `
        },
        {
            id: 'vaults',
            emoji: '💰',
            label: 'Concrete Vaults',
            content: `
                <h3>💰 concrete vaults</h3>
                <p><strong>Automated capital management systems.</strong> They reduce idle capital, auto‑compound, allocate across strategies, and minimise manual work.</p>
                <p>Vaults are financial infrastructure tools — think “programmable onchain asset managers”. They use ERC‑4626 standards and dynamic strategy deployment.</p>
                <div class="badge">🔗 <a href="https://concrete.xyz/blog-articles-list/concrete-vaults-participate-in-defi-without-becoming-a-defi-expert" target="_blank">vaults explained (blog)</a> · <a href="https://docs.concrete.xyz/Overview/how-it-works/" target="_blank">how it works</a></div>
            `
        },
        {
            id: 'app',
            emoji: '🌐',
            label: 'Concrete App',
            content: `
                <h3>🌐 concrete app – dashboard</h3>
                <p>Main interface to:</p>
                <ul><li>access vaults</li><li>track portfolio efficiency</li><li>participate in onchain strategies</li><li>monitor allocations</li></ul>
                <p>👉 launch app from official site (top right).</p>
                <p><a href="https://concrete.xyz" target="_blank">concrete.xyz</a></p>
            `
        },
        {
            id: 'points',
            emoji: '⭐',
            label: 'Points & Referral',
            content: `
                <h3>🤝 referral & points</h3>
                <p><strong>Concrete points</strong> = social tasks, discord engagement, article writing, helping others. check the points portal:</p>
                <p>🔗 <a href="https://points.concrete.xyz/profile" target="_blank">points.concrete.xyz</a></p>
                <p>Referral programs usually let you invite friends and earn recognition — always check official campaign announcements for exact rewards.</p>
                <div class="badge">💡 share your referral link in discord #referrals</div>
            `
        },
        {
            id: 'badges',
            emoji: '🏆',
            label: 'Badge levels (5,10,17,25...)',
            content: `
                <h3>🏆 badge levels</h3>
                <p>Badges reflect community participation and contribution. They recognise:</p>
                <ul><li>activity consistency</li><li>quality discussions</li><li>content creation</li><li>helping newcomers</li></ul>
                <p>Higher badge = stronger contributor recognition. Levels like 5, 10, 17, 25 … show your journey.</p>
                <p><em>No official “checklist” — genuine engagement moves you up.</em></p>
            `
        },
        {
            id: 'access',
            emoji: '🔑',
            label: '🔑 Access role',
            content: `
                <h3>🔑 acces role (how to get it)</h3>
                <p>Given to those who contributed <strong>purely and meaningfully</strong> to the community:</p>
                <ul><li>engaging in healthy conversations</li><li>making good quality content</li><li>helping others consistently</li></ul>
                <p><span class="badge">🗳️ nomination:</span> current Access holders can nominate someone they feel deserves it. If TM accepts the nomination → you receive 🔑.</p>
                <p>💬 it’s not about asking — it’s about showing up with value.</p>
            `
        },
        {
            id: 'moai',
            emoji: '🗿',
            label: '🗿 Moai role',
            content: `
                <h3>🗿 moai – most dedicated</h3>
                <p>Hand‑picked by TM (team). Given to those who:</p>
                <ul><li>help & guide others (especially newbies)</li><li>create quality content on X (twitter)</li><li>engage every day with consistency</li></ul>
                <div class="badge">🔥 my take: <em>“show your talents, put effort so team notices your work. hard work + consistency = moai.”</em></div>
                <p>no direct application — just be a pillar of the community.</p>
            `
        },
        {
            id: 'article',
            emoji: '✍️',
            label: 'Article submission (step by step)',
            content: `
                <h3>📝 how to write & submit articles</h3>
                <p><strong>if you have X premium</strong> → post thread directly on X, copy link, submit.</p>
                <p><strong>no premium? use Medium app (easy, free):</strong></p>
                <ol><li>download Medium from PlayStore</li><li>tap pencil / write icon</li><li>write your topic — keep it simple, insightful, human (not AI‑ish)</li><li>tap preview → publish</li><li>go to your profile → ⋮ three dots on article → copy link</li><li>paste link on Concrete points site or share in discord #content</li></ol>
                <div class="badge">✏️ tips: cover what matters (vaults, community, why concrete). don’t overcomplicate. help newbies understand.</div>
            `
        },
        {
            id: 'ecosystem',
            emoji: '🤝',
            label: 'Ecosystem & funding',
            content: `
                <h3>🌿 ecosystem & backup</h3>
                <p>Concrete partners with protocols like Pendle, Morpho, and more — you can explore official ecosystem page:</p>
                <p>🔗 <a href="https://concrete.xyz/ecosystem" target="_blank">concrete.xyz/ecosystem</a></p>
                <p>Funding / backup: part of long‑term infrastructure vision. not “hype funding”, but sustainable building.</p>
            `
        }
    ];

    // render buttons
    const grid = document.getElementById('buttonGrid');
    const detailDiv = document.getElementById('detailContainer');
    
    function renderButtons() {
        let html = '';
        sections.forEach(s => {
            html += `<button class="guide-btn" data-id="${s.id}">
                <span class="emoji-big">${s.emoji}</span>
                <span>${s.label}</span>
                <span class="arrow">▶</span>
            </button>`;
        });
        grid.innerHTML = html;

        // attach click events
        document.querySelectorAll('.guide-btn').forEach(btn => {
            btn.addEventListener('click', (e) => {
                const id = btn.dataset.id;
                const section = sections.find(s => s.id === id);
                if (section) {
                    detailDiv.innerHTML = `
                        <div class="detail-panel">
                            <div class="detail-content">
                                ${section.content}
                                <hr>
                                <p style="color: #42648D;"><span style="font-size:1.3rem;">💬</span> concrete is people + infra — this info is community‑gathered, always DYOR.</p>
                            </div>
                        </div>
                    `;
                    // scroll to it smoothly
                    detailDiv.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    }

    renderButtons();

    // optional: show first section as default welcome?
    window.onload = function() {
        // show a default detail maybe 'what is concrete' on load
        detailDiv.innerHTML = `
            <div class="detail-panel">
                <div class="detail-content">
                    <h3>🧱 welcome to concrete helper</h3>
                    <p>tap any button above for step‑by‑step guidance 👆</p>
                    <p style="background:#f0f9ff; padding:20px; border-radius:24px;">
                    <strong>🗣️ human note:</strong> this dapp collects what we know as a community — from acces role hints to article writing. i’m a learner like you, sharing the map.
                    </p>
                    <div class="badge">⚡ first time? start with “what is concrete” or “badge levels”</div>
                </div>
            </div>
        `;
    };
</script>
</body>
</html>
