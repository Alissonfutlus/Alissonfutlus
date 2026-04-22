<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Alisson Sorgatto | Full Stack & Mobile Architect</title>
    <!-- This snippet is designed for GitHub Profile README – uses inline styles and safe animations -->
    <style>
        /* Reset & base cosmic theme */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0b0f1c;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            font-family: 'Segoe UI', 'Ubuntu', 'Inter', system-ui, -apple-system, BlinkMacSystemFont, 'Roboto', sans-serif;
            padding: 2rem 1rem;
        }

        /* main profile card container */
        .galaxy-container {
            max-width: 1000px;
            width: 100%;
            margin: 0 auto;
            background: radial-gradient(ellipse at 30% 40%, #0f172a, #030614);
            border-radius: 3rem;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.6), 0 0 0 1px rgba(52, 152, 219, 0.2);
            overflow: hidden;
            position: relative;
            backdrop-filter: blur(2px);
            transition: all 0.3s ease;
        }

        /* animated stars background (cosmic dust) */
        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
        }

        .star {
            position: absolute;
            background-color: #ffffff;
            border-radius: 50%;
            opacity: 0.6;
            animation: twinkle 3s infinite alternate;
        }

        @keyframes twinkle {
            0% { opacity: 0.2; transform: scale(1);}
            100% { opacity: 1; transform: scale(1.2);}
        }

        /* main content relative to stars */
        .content {
            position: relative;
            z-index: 2;
            padding: 2rem 1.8rem 2rem 1.8rem;
        }

        /* header SVG section */
        .hero-svg {
            text-align: center;
            margin-bottom: 1.8rem;
        }

        /* custom styling for tech cards */
        .tech-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
            justify-content: center;
            margin: 2rem 0 1.8rem;
        }

        .glass-card {
            background: rgba(18, 25, 45, 0.65);
            backdrop-filter: blur(10px);
            border-radius: 2rem;
            padding: 1.3rem 1rem;
            width: 100%;
            max-width: 280px;
            text-align: center;
            border: 1px solid rgba(52, 152, 219, 0.3);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
            transition: transform 0.2s ease, box-shadow 0.2s;
        }

        .glass-card:hover {
            transform: translateY(-5px);
            border-color: #2ecc71;
            box-shadow: 0 18px 30px -12px rgba(46, 204, 113, 0.3);
        }

        .glass-card h3 {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            background: linear-gradient(135deg, #e0eaff, #3498db);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            letter-spacing: 1px;
        }

        .skill-icons {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 0.8rem;
            margin-top: 0.6rem;
        }

        .skill-icons img {
            width: 48px;
            height: 48px;
            transition: all 0.2s;
            filter: drop-shadow(0 2px 6px rgba(0,0,0,0.4));
        }

        .skill-icons img:hover {
            transform: scale(1.1);
            filter: drop-shadow(0 0 8px #3498db);
        }

        /* project showcase premium */
        .project-galaxy {
            background: linear-gradient(135deg, #0f212e, #07121c);
            border-radius: 3rem;
            padding: 1.5rem 1.8rem;
            margin: 1.5rem 0;
            border: 1px solid rgba(46, 204, 113, 0.5);
            box-shadow: 0 20px 35px -12px rgba(0,0,0,0.5), inset 0 1px 0 rgba(255,255,255,0.05);
            transition: all 0.3s;
        }

        .project-galaxy h2 {
            font-size: 1.9rem;
            font-weight: 800;
            background: linear-gradient(120deg, #2ecc71, #58d68d);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            letter-spacing: -0.5px;
        }

        .project-badge {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 1rem;
            justify-content: flex-start;
        }

        /* stats wrapper */
        .stats-wrapper {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .stats-card {
            background: rgba(10, 20, 30, 0.7);
            border-radius: 1.8rem;
            padding: 0.8rem;
            backdrop-filter: blur(4px);
            border: 1px solid rgba(52, 152, 219, 0.4);
            transition: all 0.2s;
        }

        .stats-card img {
            border-radius: 1.2rem;
            max-width: 100%;
            height: auto;
        }

        /* social links */
        .social-links {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.2rem;
            margin: 1.5rem 0 1rem;
        }

        .social-btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(20, 30, 45, 0.8);
            backdrop-filter: blur(5px);
            padding: 0.7rem 1.4rem;
            border-radius: 60px;
            font-weight: 600;
            text-decoration: none;
            color: #ecf0f1;
            transition: 0.25s;
            border: 1px solid rgba(52, 152, 219, 0.4);
            font-size: 1rem;
        }

        .social-btn:hover {
            transform: scale(1.05);
            background: #2c3e66;
            border-color: #3498db;
            box-shadow: 0 0 15px rgba(52,152,219,0.5);
            color: white;
        }

        /* footer wave */
        .wave-footer {
            margin-top: 1rem;
            line-height: 0;
        }

        /* responsive fine-tuning */
        @media (max-width: 700px) {
            .content {
                padding: 1.2rem;
            }
            .glass-card {
                max-width: 100%;
            }
            .project-galaxy h2 {
                font-size: 1.4rem;
            }
        }

        /* orbit animation for svg */
        @keyframes rotateOrbit {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        .orbit-ring {
            animation: rotateOrbit 20s linear infinite;
            transform-origin: 400px 100px;
        }
    </style>
</head>
<body>
<div class="galaxy-container">
    <div class="stars" id="stars-container"></div>
    <div class="content">

        <!-- Hero SVG with orbit & cosmic identity -->
        <div class="hero-svg">
            <svg width="100%" height="200" viewBox="0 0 800 200" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width: 800px; margin: 0 auto; display: block;">
                <defs>
                    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                        <stop offset="0%" stop-color="#ffffff" />
                        <stop offset="50%" stop-color="#8dd0ff" />
                        <stop offset="100%" stop-color="#2ecc71" />
                    </linearGradient>
                    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
                        <feGaussianBlur in="SourceAlpha" stdDeviation="4"/>
                        <feMerge>
                            <feMergeNode in="offsetblur" />
                            <feMergeNode in="SourceGraphic" />
                        </feMerge>
                    </filter>
                </defs>
                <circle cx="400" cy="100" r="88" stroke="#3498db" stroke-width="2.5" stroke-dasharray="10 6" class="orbit-ring" fill="none" opacity="0.9"/>
                <circle cx="400" cy="100" r="88" stroke="#2ecc71" stroke-width="1" stroke-dasharray="4 8" class="orbit-ring" fill="none" opacity="0.6" style="animation-duration: 28s; animation-direction: reverse;"/>
                <text x="50%" y="45%" dominant-baseline="middle" text-anchor="middle" font-family="'Segoe UI', Ubuntu, Sans-Serif" font-weight="800" font-size="44" fill="url(#nameGrad)" filter="url(#glow)" letter-spacing="2">ALISSON SORGATTO</text>
                <text x="50%" y="68%" dominant-baseline="middle" text-anchor="middle" font-family="'Segoe UI', Ubuntu, Sans-Serif" font-weight="600" font-size="19" fill="#4cc9f0" letter-spacing="4" text-transform="uppercase">Full Stack & Mobile Architect</text>
                <circle cx="320" cy="100" r="4" fill="#2ecc71" opacity="0.9">
                    <animate attributeName="opacity" values="0.3;1;0.3" dur="2s" repeatCount="indefinite" />
                </circle>
                <circle cx="480" cy="100" r="3.5" fill="#3498db" opacity="0.8">
                    <animate attributeName="r" values="2;5;2" dur="3s" repeatCount="indefinite" />
                </circle>
            </svg>
        </div>

        <!-- Tech Stack & Hardware with glassmorphic cards (2 column vibe) -->
        <div class="tech-grid">
            <!-- Left: Tech Stack Cosmos -->
            <div class="glass-card">
                <h3>🚀 TECH STACK COSMOS</h3>
                <div class="skill-icons">
                    <img src="https://skillicons.dev/icons?i=react" alt="React" />
                    <img src="https://skillicons.dev/icons?i=expo" alt="Expo" />
                    <img src="https://skillicons.dev/icons?i=nodejs" alt="Node.js" />
                    <img src="https://skillicons.dev/icons?i=mongodb" alt="MongoDB" />
                    <img src="https://skillicons.dev/icons?i=js" alt="JavaScript" />
                    <img src="https://skillicons.dev/icons?i=ts" alt="TypeScript" />
                </div>
            </div>
            <!-- Right: Live Ops & Hardware -->
            <div class="glass-card">
                <h3>🎥 LIVE OPS & HARDWARE</h3>
                <div class="skill-icons">
                    <img src="https://skillicons.dev/icons?i=obs" alt="OBS" />
                    <img src="https://skillicons.dev/icons?i=arduino" alt="Arduino" />
                    <img src="https://skillicons.dev/icons?i=raspberrypi" alt="Raspberry Pi" />
                    <img src="https://skillicons.dev/icons?i=redhat" alt="RedHat" />
                    <img src="https://skillicons.dev/icons?i=linux" alt="Linux" />
                    <img src="https://skillicons.dev/icons?i=github" alt="GitHub" />
                </div>
            </div>
        </div>

        <!-- PROJETO GALAXY: FUT+ enhanced -->
        <div class="project-galaxy">
            <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center;">
                <h2>⚽ PROJETO GALAXY: FUT+</h2>
                <div class="project-badge">
                    <img src="https://img.shields.io/badge/Status-Publicado_Store-brightgreen?style=for-the-badge&logo=apple&color=2ecc71" alt="status store" />
                    <img src="https://img.shields.io/badge/Engine-React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React Native" />
                </div>
            </div>
            <p style="color: #cbd5e6; font-size: 1.05rem; margin-top: 12px; line-height: 1.4;">🌟 Plataforma completa de gestão esportiva e transmissões ao vivo. Integração com IoT, analytics em tempo real e experiência mobile-first.</p>
            <div style="margin-top: 15px; display: flex; gap: 12px; flex-wrap: wrap;">
                <span style="background: #1f3a4b; padding: 5px 12px; border-radius: 40px; font-size: 0.75rem; color:#bbf0ff;">📱 Mobile & TV</span>
                <span style="background: #1f3a4b; padding: 5px 12px; border-radius: 40px; font-size: 0.75rem; color:#bbf0ff;">🕹️ Live Overlay</span>
                <span style="background: #1f3a4b; padding: 5px 12px; border-radius: 40px; font-size: 0.75rem; color:#bbf0ff;">📊 Advanced Metrics</span>
            </div>
        </div>

        <!-- GitHub Stats with modern glass style -->
        <div class="stats-wrapper">
            <div class="stats-card">
                <img height="180em" src="https://github-readme-stats.vercel.app/api?username=alissonsorgatto&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=1a252f&title_color=3498db&icon_color=2ecc71&ring_color=2ecc71" alt="github stats" />
            </div>
            <div class="stats-card">
                <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=alissonsorgatto&layout=compact&theme=tokyonight&hide_border=true&bg_color=1a252f&title_color=3498db&text_color=cdd9f4" alt="top languages" />
            </div>
        </div>

        <!-- Social links with beautiful interactive buttons -->
        <div class="social-links">
            <a href="#" class="social-btn" target="_blank">
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C0.792 0 0 0.774 0 1.729v20.542C0 23.227 0.792 24 1.771 24h20.451c0.979 0 1.771-0.773 1.771-1.729V1.729C24 0.774 23.205 0 22.225 0z"/></svg>
                LinkedIn
            </a>
            <a href="#" class="social-btn" target="_blank">
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z"/></svg>
                Instagram
            </a>
            <a href="mailto:alisson.sorgatto@example.com" class="social-btn" target="_blank">
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
                Gmail
            </a>
            <a href="#" class="social-btn" target="_blank">
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.302 3.438 9.8 8.205 11.387.6.113.82-.26.82-.58 0-.287-.01-1.05-.015-2.06-3.338.726-4.042-1.416-4.042-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.082-.73.082-.73 1.205.085 1.838 1.237 1.838 1.237 1.07 1.834 2.807 1.304 3.492.997.108-.775.418-1.305.762-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.468-2.38 1.235-3.22-.123-.3-.535-1.52.117-3.16 0 0 1.008-.322 3.3 1.23.96-.267 1.98-.4 3-.405 1.02.005 2.04.138 3 .405 2.29-1.552 3.297-1.23 3.297-1.23.653 1.64.24 2.86.118 3.16.768.84 1.233 1.91 1.233 3.22 0 4.61-2.804 5.62-5.476 5.92.43.37.824 1.102.824 2.22 0 1.602-.015 2.894-.015 3.287 0 .322.216.698.83.578C20.565 21.795 24 17.3 24 12c0-6.63-5.37-12-12-12z"/></svg>
                GitHub
            </a>
        </div>

        <!-- additional cosmic message line -->
        <div style="text-align: center; margin: 1.8rem 0 0.5rem;">
            <span style="background: linear-gradient(90deg, #1f3e48, #0f1a24); padding: 0.4rem 1rem; border-radius: 60px; font-size: 0.8rem; color: #9cc9f0;">✨ "Building the future, one commit at a time" ✨</span>
        </div>
    </div>

    <!-- Animated wave footer (capsule render but with custom style) -->
    <div class="wave-footer">
        <svg width="100%" height="70" viewBox="0 0 1200 120" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0,64L80,58.7C160,53,320,43,480,48C640,53,800,75,960,80C1120,85,1280,75,1360,69.3L1440,64L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z" fill="#0d2b3e" fill-opacity="0.9"></path>
            <path d="M0,96L80,90.7C160,85,320,75,480,80C640,85,800,107,960,106.7C1120,107,1280,96,1360,90.7L1440,85L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z" fill="#05161f" fill-opacity="0.7"></path>
            <path d="M0,106L80,101.3C160,96,320,85,480,90.7C640,96,800,117,960,117.3C1120,117,1280,107,1360,101.3L1440,96L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z" fill="#030d13"></path>
        </svg>
    </div>
</div>

<script>
    // Generate random twinkling stars for cosmic background effect
    function createStars() {
        const starsContainer = document.getElementById('stars-container');
        if (!starsContainer) return;
        const starCount = 130;
        for (let i = 0; i < starCount; i++) {
            const star = document.createElement('div');
            star.classList.add('star');
            const size = Math.random() * 2.5 + 0.8;
            star.style.width = `${size}px`;
            star.style.height = `${size}px`;
            star.style.left = `${Math.random() * 100}%`;
            star.style.top = `${Math.random() * 100}%`;
            star.style.animationDelay = `${Math.random() * 4}s`;
            star.style.animationDuration = `${Math.random() * 2 + 1.5}s`;
            star.style.opacity = Math.random() * 0.6 + 0.2;
            starsContainer.appendChild(star);
        }
    }
    createStars();
</script>

<!-- Optional: ensure that the links are updated by the user, but design is pristine and interactive -->
<!-- GitHub username in stats uses "alissonsorgatto" as placeholder – you can replace with your actual username -->
</body>
</html>
