<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toxic Labs: From Digital Chaos to Artistic Vision</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #16213e 100%);
            color: #ffffff;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .hero {
            text-align: center;
            padding: 80px 0;
            position: relative;
        }

        .hero h1 {
            font-size: 4rem;
            font-weight: bold;
            background: linear-gradient(45deg, #ff1493, #00ffff, #ff6b6b);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 20px;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
        }

        .subtitle {
            font-size: 1.5rem;
            color: #b0b0b0;
            margin-bottom: 40px;
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin: 30px 0;
            flex-wrap: wrap;
        }

        .hero-stat {
            text-align: center;
            padding: 15px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            min-width: 120px;
        }

        .hero-stat .stat-number {
            display: block;
            font-size: 2rem;
            font-weight: bold;
            background: linear-gradient(45deg, #ff1493, #00ffff);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-stat .stat-label {
            display: block;
            font-size: 0.8rem;
            color: #b0b0b0;
            margin-top: 5px;
        }

        .cta-buttons {
            margin-top: 40px;
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .cta-primary, .cta-secondary {
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }

        .cta-primary {
            background: linear-gradient(45deg, #ff1493, #00ffff);
            color: #000;
        }

        .cta-secondary {
            background: transparent;
            color: #00ffff;
            border: 2px solid #00ffff;
        }

        .cta-primary:hover, .cta-secondary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(255, 20, 147, 0.4);
        }

        .section {
            margin: 80px 0;
            padding: 40px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .section-header {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
        }

        .section-number {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(45deg, #ff1493, #00ffff);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: bold;
            margin-right: 20px;
            color: #000;
        }

        .section h2 {
            font-size: 2.5rem;
            color: #ffffff;
            margin-bottom: 10px;
        }

        .section h3 {
            font-size: 1.2rem;
            color: #00ffff;
            font-weight: normal;
            opacity: 0.8;
        }

        .content {
            line-height: 1.8;
            font-size: 1.1rem;
        }

        .highlight-box {
            background: linear-gradient(135deg, rgba(255, 20, 147, 0.2), rgba(0, 255, 255, 0.2));
            padding: 25px;
            border-radius: 15px;
            margin: 20px 0;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .platform-showcase {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .platform-card {
            background: rgba(0, 0, 0, 0.4);
            border-radius: 20px;
            padding: 25px;
            text-align: center;
            transition: all 0.4s ease;
        }

        .zora-card {
            border: 2px solid rgba(138, 43, 226, 0.5);
            background: linear-gradient(135deg, rgba(138, 43, 226, 0.1), rgba(75, 0, 130, 0.1));
        }

        .pumpfun-card {
            border: 2px solid rgba(255, 165, 0, 0.5);
            background: linear-gradient(135deg, rgba(255, 165, 0, 0.1), rgba(255, 140, 0, 0.1));
        }

        .platform-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(255, 20, 147, 0.3);
        }

        .platform-icon {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .platform-subtitle {
            color: #00ffff;
            font-size: 0.9rem;
            font-style: italic;
        }

        .contract-info {
            margin: 15px 0;
            padding: 15px;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            border: 1px solid rgba(138, 43, 226, 0.3);
        }

        .contract-address {
            font-size: 0.7rem;
            color: #8a2be2;
            font-family: monospace;
            word-break: break-all;
        }

        .verification-badge {
            margin: 15px 0;
            padding: 10px;
            background: rgba(0, 255, 0, 0.1);
            border: 1px solid rgba(0, 255, 0, 0.3);
            border-radius: 8px;
            font-size: 0.9rem;
        }

        .platform-link {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background: linear-gradient(45deg, #8a2be2, #4b0082);
            color: #fff;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .pumpfun-card .platform-link {
            background: linear-gradient(45deg, #ffa500, #ff8c00);
            color: #000;
        }

        .ecosystem-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .stat-number {
            font-size: 3rem;
            font-weight: bold;
            background: linear-gradient(45deg, #ff1493, #00ffff);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
        }

        .nft-showcase {
            margin: 40px 0;
        }

        .market-stats {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .stat-highlight {
            background: rgba(255, 20, 147, 0.2);
            padding: 10px 20px;
            border-radius: 25px;
            font-size: 0.9rem;
            border: 1px solid rgba(255, 20, 147, 0.5);
        }

        .nft-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .nft-card {
            background: rgba(0, 0, 0, 0.4);
            border-radius: 20px;
            padding: 20px;
            text-align: center;
            border: 2px solid rgba(255, 20, 147, 0.3);
            transition: all 0.4s ease;
            cursor: pointer;
        }

        .nft-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 25px 50px rgba(255, 20, 147, 0.4);
        }

        .nft-image-placeholder {
            width: 100%;
            height: 200px;
            background: linear-gradient(135deg, rgba(255, 20, 147, 0.3), rgba(0, 255, 255, 0.3));
            border-radius: 15px;
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        .nft-preview {
            font-size: 4rem;
            filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.5));
        }

        .nft-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.8);
            color: #00ffff;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            opacity: 0;
            transition: all 0.3s ease;
            border-radius: 15px;
        }

        .nft-card:hover .nft-overlay {
            opacity: 1;
        }

        .nft-card h4 {
            color: #ffffff;
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .nft-card p {
            color: #b0b0b0;
            font-size: 0.9rem;
            line-height: 1.4;
        }

        .trust-signals {
            margin: 40px 0;
            padding: 30px;
            background: rgba(255, 255, 255, 0.02);
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .trust-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .trust-item {
            padding: 20px;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            border-left: 4px solid #00ffff;
        }

        .roadmap-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .roadmap-item {
            background: rgba(255, 255, 255, 0.05);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }

        .roadmap-item:hover {
            transform: translateY(-5px);
            background: rgba(255, 20, 147, 0.1);
        }

        .roadmap-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .contact-card {
            background: rgba(0, 0, 0, 0.3);
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }

        .contact-card:hover {
            transform: translateY(-10px);
            background: rgba(255, 20, 147, 0.1);
        }

        .zora-focused {
            border: 2px solid rgba(138, 43, 226, 0.3);
        }

        .pumpfun-focused {
            border: 2px solid rgba(255, 165, 0, 0.3);
        }

        .investor-focused {
            border: 2px solid rgba(0, 255, 255, 0.3);
        }

        .action-link {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background: linear-gradient(45deg, #ff1493, #00ffff);
            color: #000;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .action-link:hover {
            transform: scale(1.05);
        }

        .platform-disclaimer {
            background: rgba(255, 165, 0, 0.1);
            border: 1px solid rgba(255, 165, 0, 0.3);
            border-radius: 15px;
            padding: 25px;
            margin: 30px 0;
            text-align: center;
        }

        .platform-disclaimer h4 {
            color: #ffa500;
            margin-bottom: 15px;
        }

        .social-links {
            text-align: center;
            margin-top: 50px;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        .social-grid {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .social-link {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 10px 20px;
            background: rgba(255, 255, 255, 0.05);
            color: #ffffff;
            text-decoration: none;
            border-radius: 25px;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .social-link:hover {
            background: rgba(0, 255, 255, 0.2);
            transform: translateY(-3px);
        }

        .tagline {
            text-align: center;
            font-size: 1.5rem;
            font-style: italic;
            color: #00ffff;
            margin: 60px 0;
            padding: 30px;
            background: rgba(0, 255, 255, 0.1);
            border-radius: 15px;
            border: 1px solid rgba(0, 255, 255, 0.3);
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            .section {
                padding: 20px;
                margin: 40px 0;
            }
            .section h2 {
                font-size: 2rem;
            }
            .hero-stats {
                gap: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="hero">
            <h1>TOXIC LABS</h1>
            <p class="subtitle">From Digital Chaos to Artistic Vision</p>
            <div class="hero-stats">
                <div class="hero-stat">
                    <span class="stat-number">101</span>
                    <span class="stat-label">Verified Zora Pieces</span>
                </div>
                <div class="hero-stat">
                    <span class="stat-number">$5.14K</span>
                    <span class="stat-label">Pump.fun Success</span>
                </div>
                <div class="hero-stat">
                    <span class="stat-number">2</span>
                    <span class="stat-label">Platform Ecosystem</span>
                </div>
            </div>
            <div class="cta-buttons">
                <a href="#collection" class="cta-primary">View Collection</a>
                <a href="#contact" class="cta-secondary">Partner With Us</a>
            </div>
        </div>

        <div class="section">
            <div class="section-header">
                <div class="section-number">I</div>
                <div>
                    <h2>Genesis</h2>
                    <h3>Born from the Digital Underbelly</h3>
                </div>
            </div>
            <div class="content">
                <div class="highlight-box">
                    <strong>The Spark:</strong> Toxic Labs emerged from a universal frustration—the relentless tide of online scams, phishing attempts, and digital deception that plague our connected world. Rather than simply complaining about these digital parasites, we asked: what if we gave them form?
                </div>
                <p><strong>Genesis Foundation on Zora:</strong> Our journey began with establishing a serious artistic foundation. With 101 carefully curated pieces on Zora, we built our core collection—transforming abstract digital threats into structured, collectible art that demonstrates our long-term commitment to this vision.</p>
                
                <div class="platform-showcase">
                    <div class="platform-card zora-card">
                        <div class="platform-icon">🎨</div>
                        <h4>Genesis Collection on Zora</h4>
                        <span class="platform-subtitle">Our Artistic Foundation</span>
                        <p>101 foundational pieces establishing Toxic Labs as a serious artistic endeavor</p>
                        <div class="contract-info">
                            <div class="contract-address">
                                Contract: 0x1d93...b4f62
                            </div>
                        </div>
                        <a href="https://zora.co/collect/eth:0x1d930ee342e1f057ac4e2f8a2c930a9bf06b4f62" class="platform-link">Explore Genesis →</a>
                    </div>
                    
                    <div class="platform-card pumpfun-card">
                        <div class="platform-icon">⚡</div>
                        <h4>Creature Features on Pump.fun</h4>
                        <span class="platform-subtitle">Limited, Dynamic Editions</span>
                        <p>Unleashing the untamed chaos - playful, speculative manifestations of digital threats</p>
                        <div class="verification-badge">
                            ✅ Verified Creator with Zora History
                        </div>
                        <a href="https://pump.fun/toxiclabs" class="platform-link">Unleash Chaos →</a>
                    </div>
                </div>
            </div>
        </div>

        <div class="section">
            <div class="section-header">
                <div class="section-number">II</div>
                <div>
                    <h2>Dual-Platform Evolution</h2>
                    <h3>From Structured Art to Dynamic Chaos</h3>
                </div>
            </div>
            <div class="content">
                <p><strong>The Zora Foundation:</strong> Our artistic journey began with building credibility and demonstrating long-term commitment. With 101 pieces on Zora, we established Toxic Labs as more than just a concept—we created a legitimate artistic ecosystem with proven community engagement and verified provenance.</p>
                
                <div class="highlight-box">
                    <strong>Proven Market Success:</strong> From our established Zora roots, we've expanded to Pump.fun where our Toxic Tricksters collection has reached $5.14K per NFT. This dual-platform strategy leverages artistic credibility while embracing the dynamic, speculative energy of emerging markets.
                </div>
                
                <p><strong>Strategic Differentiation:</strong> Our Zora collection represents the structured transformation of digital chaos into art, while our Pump.fun "Creature Features" embody the raw, untamed chaos that inspired our original vision. Together, they create a complete ecosystem spanning artistic legitimacy and speculative innovation.</p>

                <div class="ecosystem-stats">
                    <div class="stat-card">
                        <div class="stat-number">101</div>
                        <h4>Zora Genesis</h4>
                        <p>Foundational pieces establishing artistic credibility</p>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">$5.14K</div>
                        <h4>Pump.fun Value</h4>
                        <p>Per Toxic Trickster NFT</p>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">∞</div>
                        <h4>Cross-Platform</h4>
                        <p>Unified Toxic Labs ecosystem</p>
                    </div>
                </div>
                
                <div class="nft-showcase" id="collection">
                    <h4 style="text-align: center; margin: 30px 0; color: #00ffff;">Featured Toxic Tricksters Collection</h4>
                    <div class="market-stats">
                        <div class="stat-highlight">🎨 Built on Zora Foundation</div>
                        <div class="stat-highlight">⚡ Active on Pump.fun</div>
                        <div class="stat-highlight">📈 Cross-Platform Success</div>
                    </div>
                    <div class="nft-grid">
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">💀</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>Grin Venom</h4>
                            <p>The skeletal trickster spreading digital decay through infected networks</p>
                        </div>
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">👁️</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>One Eyed Willy</h4>
                            <p>The golden-spotted predator hunting for unsuspecting victims</p>
                        </div>
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">🐍</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>Fishy Phillip</h4>
                            <p>The serpentine data harvester with tentacles reaching across cyberspace</p>
                        </div>
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">🦠</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>Pandemic Puff</h4>
                            <p>The viral spreader contaminating global digital ecosystems</p>
                        </div>
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">😵</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>Glitch This Shit</h4>
                            <p>The deceptive worm hiding malicious code behind innocent smiles</p>
                        </div>
                        <div class="nft-card">
                            <div class="nft-image-placeholder">
                                <div class="nft-preview">🌐</div>
                                <div class="nft-overlay">
                                    <div>View on Pump.fun</div>
                                    <div class="nft-price">$5.14K</div>
                                </div>
                            </div>
                            <h4>Malice Mire</h4>
                            <p>The cosmic entity orchestrating digital chaos across multiple dimensions</p>
                        </div>
                    </div>
                </div>

                <div class="trust-signals">
                    <h4>Why This Strategy Works</h4>
                    <div class="trust-grid">
                        <div class="trust-item">
                            <strong>🎨 Verified Provenance</strong>
                            <p>Contract 0x1d93...b4f62 - 101 pieces on Zora proving sustained commitment</p>
                        </div>
                        <div class="trust-item">
                            <strong>📈 Market Validation</strong>
                            <p>$5.14K Pump.fun success backed by established Zora foundation</p>
                        </div>
                        <div class="trust-item">
                            <strong>🔗 Transparent Provenance</strong>
                            <p>On-chain history across platforms creates verifiable digital identity</p>
                        </div>
                        <div class="trust-item">
                            <strong>🌱 Sustainable Growth</strong>
                            <p>Dual-platform strategy balances stability with innovation</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="section">
            <div class="section-header">
                <div class="section-number">III</div>
                <div>
                    <h2>Cross-Platform Roadmap</h2>
                    <h3>Expanding the Toxic Labs Ecosystem</h3>
                </div>
            </div>
            <div class="content">
                <div class="roadmap-grid">
                    <div class="roadmap-item">
                        <div class="roadmap-icon">🎯</div>
                        <h4>Q4 2025</h4>
                        <p><strong>Zora Expansion:</strong> Launch "Genesis II" collection - 50 new foundational pieces exploring deeper digital threat concepts</p>
                    </div>
                    <div class="roadmap-item">
                        <div class="roadmap-icon">⚡</div>
                        <h4>Q1 2026</h4>
                        <p><strong>Pump.fun Chaos Series:</strong> Release limited-edition "Viral Outbreak" creatures with dynamic pricing and community governance</p>
                    </div>
                    <div class="roadmap-item">
                        <div class="roadmap-icon">🤝</div>
                        <h4>Q2 2026</h4>
                        <p><strong>Cross-Platform Integration:</strong> Bridge holders get exclusive access to collections on both platforms</p>
                    </div>
                    <div class="roadmap-item">
                        <div class="roadmap-icon">🏪</div>
                        <h4>Q3 2026</h4>
                        <p><strong>Physical Manifestation:</strong> Limited edition sculptures for Zora Genesis holders, Pump.fun creature toys</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="section" id="contact">
            <div class="section-header">
                <div class="section-number">IV</div>
                <div>
                    <h2>Join the Ecosystem</h2>
                    <h3>Choose Your Level of Chaos</h3>
                </div>
            </div>
            <div class="content">
                <div class="contact-grid">
                    <div class="contact-card zora-focused">
                        <h4>🎨 Serious Collectors</h4>
                        <p>Explore our established Genesis Collection on Zora - 101 verified pieces of foundational digital threat art</p>
                        <small style="color: #8a2be2; font-family: monospace;">Contract: 0x1d93...b4f62</small>
                        <a href="https://zora.co/collect/eth:0x1d930ee342e1f057ac4e2f8a2c930a9bf06b4f62" class="action-link">Browse Zora Genesis</a>
                    </div>
                    <div class="contact-card pumpfun-focused">
                        <h4>⚡ Chaos Seekers</h4>
                        <p>Unleash the dynamic energy with our Pump.fun Creature Features - speculative, playful manifestations</p>
                        <a href="https://pump.fun/toxiclabs" class="action-link">Unleash on Pump.fun</a>
                    </div>
                    <div class="contact-card investor-focused">
                        <h4>💼 Strategic Partners</h4>
                        <p>Join our cross-platform vision transforming digital threats into sustainable art ecosystems</p>
                        <a href="mailto:hello@toxiclabs.art" class="action-link">Partner With Us</a>
                    </div>
                </div>
                
                <div class="platform-disclaimer">
                    <h4>⚠️ Platform Transparency & Risk Disclosure</h4>
                    <p><strong>Zora Foundation:</strong> Our artistic foundation with established provenance, long-term collecting focus, and verified on-chain history (Contract: 0x1d93...b4f62).</p>
                    <p><strong>Pump.fun Experimentation:</strong> Speculative tokens designed for dynamic engagement with our chaos theme. Higher risk, experimental nature - not financial advice. These represent authentic artistic expression aligned with our brand, but understand the speculative nature of this platform.</p>
                    <p><strong>Unified Vision:</strong> Both platforms serve different collector preferences while maintaining authentic Toxic Labs identity. We're transparent about each platform's characteristics and encourage informed participation.</p>
                </div>
                
                <div class="social-links">
                    <h4>Follow Our Cross-Platform Evolution</h4>
                    <div class="social-grid">
                        <a href="https://zora.co/collect/eth:0x1d930ee342e1f057ac4e2f8a2c930a9bf06b4f62" class="social-link">
                            <span>🎨</span>
                            <span>Zora Genesis</span>
                        </a>
                        <a href="https://pump.fun/toxiclabs" class="social-link">
                            <span>⚡</span>
                            <span>Pump.fun Chaos</span>
                        </a>
                        <a href="https://twitter.com/toxiclabs" class="social-link">
                            <span>🐦</span>
                            <span>Twitter</span>
                        </a>
                        <a href="https://discord.gg/toxiclabs" class="social-link">
                            <span>💬</span>
                            <span>Discord</span>
                        </a>
                    </div>
                </div>
            </div>
        </div>

        <div class="tagline">
            "Toxic Labs transforms digital age anxieties into compelling art, creating a unique intersection of social commentary and collectible creativity."
        </div>
    </div>

    <script>
        // Smooth scrolling for anchor links
        document.addEventListener('DOMContentLoaded', function() {
            var links = document.querySelectorAll('a[href^="#"]');
            for (var i = 0; i < links.length; i++) {
                links[i].addEventListener('click', function(e) {
                    e.preventDefault();
                    var target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth'
                        });
                    }
                });
            }
        });

        // Simple hover effects for NFT cards
        document.addEventListener('DOMContentLoaded', function() {
            var nftCards = document.querySelectorAll('.nft-card');
            for (var i = 0; i < nftCards.length; i++) {
                nftCards[i].addEventListener('mouseenter', function() {
                    this.style.background = 'rgba(255, 20, 147, 0.15)';
                });
                nftCards[i].addEventListener('mouseleave', function() {
                    this.style.background = 'rgba(0, 0, 0, 0.4)';
                });
            }
        });
    </script>
</body>
</html>
