# 💻 Hi, I'm **Arpit Bansal** 🚀

╔═══════════════════════════════════════════════╗
║   FULL-STACK DEVELOPER | WEB3 ENTHUSIAST     ║
║   React • TypeScript • Three.js • Node.js     ║
║   📍 Pune, India | 💼 @Amdocs               ║
╚═══════════════════════════════════════════════╝

---

## 🎯 **About**

I'm a passionate software developer specializing in **modern web applications**, **real-time systems**, and **emerging technologies**. I build scalable architectures, craft delightful user experiences, and push the boundaries of what's possible on the web.

**Current Focus:**
- 🎨 **Frontend:** React 18, TypeScript, GSAP animations, Three.js WebGL
- ⚙️ **Backend:** Node.js, Express, REST APIs, serverless functions
- 🌐 **Web3:** Smart contracts, NFTs, blockchain integration
- 🎬 **Real-Time:** Live streaming (RTMP), WebSockets, media servers
- 📊 **Architecture:** RTK Query, Redux normalization, BFF patterns

---

## 💼 **Professional Experience**

**Software Developer @ Amdocs** (Pune, India)  
*Building production tools and optimizing developer workflows*

**Key Achievements:**
- 🔧 Built 5+ production tools: ComcastHub, BPT Charge, Cipher EOC, APEye, CSL Auction
- ⚡ **90% Manual Work Reduction** via intelligent automation
- 📈 **5h → 1h** Test cycle optimization with Jenkins orchestration
- 🎯 **15-20% Productivity Boost** through unified dev tools
- 🚀 **10+ Developer Use Cases** powered with API regression tools

---

## 🏆 **Featured Projects**

### 🌐 **Portfolio Website** — *Production Showcase*
> Modern, scroll-driven portfolio with 3D tech stack visualization

**Architecture:**
- **Stack:** React 18 + TypeScript + Vite
- **Animations:** GSAP ScrollTrigger, ScrollSmoother, SplitText
- **3D:** Three.js + React Three Fiber + Rapier physics
- **Deploy:** Netlify (static + serverless forms)

**Key Features:**
✨ Scroll-driven animations 🎮 Interactive 3D tech stack with physics 📱 Mobile-first responsive design 🎯 SEO optimized (JSON-LD schema) ⚡ Vite for fast HMR & code splitting 🎨 Data-driven from portfolio.ts


**Performance Wins:**
- Code splitting: `lazy(MainContainer)`, `lazy(TechStack)`
- Cache busting with version timestamps
- Netlify headers for asset caching
- ScrollSmoother disabled on mobile (<1024px)

[→ Explore Repository](https://github.com/ArpitBansal047/Portfolio-Website)

---

### 💰 **Cryptoverse** — *Crypto Dashboard SPA*
> Real-time cryptocurrency explorer with multi-API aggregation

**Architecture:**
- **State Management:** Redux Toolkit Query (RTK Query)
- **APIs:** Coinranking (RapidAPI), CoinGecko (free), Google News RSS
- **Caching:** Built-in RTK Query deduplication + 5min serverless TTL
- **Deploy:** Netlify (static + serverless function for CORS)

**Key Patterns:**
📊 Separate RTK Query slices per provider 🔄 Custom baseQuery for news fallback chain 💾 Automatic cache sharing (Homepage + Cryptocurrencies) 📈 Chart.js v3 for price history visualization 🌐 Netlify function as transparent CORS proxy


**Technical Depth:**
- Client-side search over 100 coins
- Parallel queries for details + history
- Multi-source fallback: Google News RSS → GNews.io
- RapidAPI optimization (removed Coinranking for exchanges)

**Bottlenecks Identified (10x load):**
❌ Rate limits: RapidAPI free tier caps ❌ Client-side fetch: Doesn't scale ❌ Single news point: Need circuit breaker pattern ✅ Fix: Server-side cache layer (Redis) + API key management


[→ Explore Repository](https://github.com/ArpitBansal047/Cryptoverse)

---

### 🎮 **Cyberpunks** — *NFT Collectibles*
> Blockchain-integrated Web3 application

**Architecture:**
- **Web3:** Ethers.js, MetaMask wallet integration
- **Smart Contracts:** OpenZeppelin standards (ERC-721)
- **IPFS:** Metadata storage
- **Frontend:** React + Web3 hooks

**Key Features:** 
🔗 Live blockchain interaction 👛 MetaMask wallet connect 🎨 NFT gallery & metadata display ⛓️ Smart contract support


[→ Explore Repository](https://github.com/ArpitBansal047/Cyberpunks)

---

### 🎥 **Streamer** — *Live Streaming Platform*
> Full-stack Twitch-inspired streaming application

**Architecture:**
┌─────────────────────┐ REST CRUD ┌─────────────────────┐ │ React Client │ ←───────────────→ │ json-server │ │ CRA, port 3000 │ │ port 3001 │ │ Redux + Router v5 │ │ db.json (file DB) │ └──────────┬──────────┘ └─────────────────────┘ │ HTTP-FLV playback ▼ ┌─────────────────────┐ RTMP ingest ┌─────────────────────┐ │ flv.js player │ ←─────────────── │ node-media-server │ │ (browser) │ :8000/live/{id} │ RTMP :1935 │ └─────────────────────┘ └──────────▲──────────┘ │ OBS Studio


**Tech Stack:**
- **Frontend:** React 16 + Redux + Redux-Form
- **Media Server:** node-media-server (RTMP → HTTP-FLV)
- **API:** json-server (mock REST)
- **Playback:** flv.js for low-latency browser streaming
- **Auth:** Google OAuth

**Design Patterns:**
🎬 Normalized Redux state (O(1) lookup by stream id) 🔄 Redux-Form HOC for create/edit 📱 Programmatic navigation via history module 🎯 Class lifecycle for FLV player cleanup


**Production Gaps (10x load):**
❌ File-based DB → PostgreSQL + Express + JWT ❌ RTMP on static host → Dedicated VPS/K8s ❌ flv.js only → Add HLS (hls.js) for mobile ❌ Single origin → CDN edge caching + multi-region ✅ Solution: Origin + CDN (CloudFront), SRS clustering


[→ Explore Repository](https://github.com/ArpitBansal047/Streamer)

---

### 🎓 **Thapar Website** — *Educational Portal*
> Responsive university information hub

**Tech:** HTML5, CSS3, JavaScript, GitHub Pages ready

[→ Explore Repository](https://github.com/ArpitBansal047/Thapar_Website)

---

### 📱 **RavenSwift** — *Social Media Design*
> Beautiful UI/UX for social networking

**Design Focus:** Material Design 3, smooth animations, accessibility

[→ Explore Repository](https://github.com/ArpitBansal047/Ravenswift)

---

## 🛠️ **Technical Arsenal**

### Languages & Frameworks
```javascript
// Frontend Mastery
React 18 | TypeScript | Vite | Redux Toolkit
GSAP | Three.js | Tailwind CSS

// Backend Capabilities  
Node.js | Express | REST APIs | Serverless Functions

// Web3 & Streaming
Web3.js | Ethers.js | RTMP | WebSockets | FLV.js

// Tools & DevOps
Git | GitHub Actions | Netlify | Docker

✅ RTK Query caching & deduplication
✅ Redux normalization (mapKeys, omit)
✅ BFF-lite with serverless proxies
✅ Custom baseQuery for multi-source fallbacks
✅ Scroll-driven animations (GSAP)
✅ Code splitting & lazy loading
✅ Responsive design (mobile-first)
✅ SEO optimization (JSON-LD)

<div align="center">
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=ArpitBansal047&theme=tokyonight&hide_border=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ArpitBansal047&theme=tokyonight&hide_border=true&layout=compact)

</div>
🎓 Education
Thapar University, Patiala
Engineering Degree • Computer Science Foundation

🌱 Continuously Learning
🔬 Advanced React patterns & performance optimization
🎨 3D web experiences (Babylon.js, p5.js)
⛓️ Smart contract development (Solidity)
📡 Real-time protocols (WebRTC, HLS)
🚀 DevOps & infrastructure as code
💡 Interview Talking Points (3+ YOE)
Architecture Decisions

Q: "Why RTK Query over Redux Thunk?"
A: Automatic caching, deduplication, loading/error states.
   Homepage and list page share cache key — one network request.

Q: "How do you handle CORS?"
A: Dev: setupProxy. Prod: Netlify serverless function as 
   transparent proxy with Cache-Control headers.

Q: "Multi-API strategy?"
A: Separate RTK slices per provider (different base URLs, headers).
   Custom baseQuery for fallback chain (primary → secondary → tertiary).

Q: "Scale from 1x to 10x load?"
A: Static assets: Netlify CDN handles. API rate limits hit first —
   need backend cache layer (Redis) aggregating with TTL.

Performance Optimization
✨ Code splitting: lazy() for large chunks
⚡ Cache busting: version timestamps
📦 Bundle analysis: webpack-bundle-analyzer
🎯 Lazy hydration: ScrollTrigger for animations

Web3 & Streaming

🔗 Ethers.js for contract interaction
🎬 RTMP ingest, HTTP-FLV playback
📡 WebSocket for real-time updates

 Let's Connect!
<div align="center">
![GitHub](https://img.shields.io/badge/GitHub-ArpitBansal047-181717?style=for-the-badge&logo=github&logoColor=white) ![LinkedIn](https://img.shields.io/badge/LinkedIn-arpit0291-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white) ![Email](https://img.shields.io/badge/Email-bansal.arpit02@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white) ![Portfolio](https://img.shields.io/badge/Portfolio-arpit--bansal-6200EE?style=for-the-badge&logo=react&logoColor=white)

</div>
🎯 Open To Opportunities
🔧 Roles: Full-Stack Engineer, Frontend Architect, Web3 Developer
💬 Collaboration: Open-source, freelance, startup projects
📧 Contact: bansal.arpit02@gmail.com
<div align="center">
⭐ If you find my work interesting, star my repositories!
  _____  _             _     ____                    _ 
 |  _  || |           | |   |  _ \                  | |
 | |_| || |  _   _  __| |   | |_) |  ___   _ __   __| |
 |  _  || | | | | |/ _` |   |  _ <  / _ \ | '_ \ / _` |
 | | | || | | |_| | (_| |   | |_) || (_) || | | | (_| |
 |_| |_||_|  \__,_|\__,_|   |____/  \___/ |_| |_|\__,_|

Made with ❤️ by Arpit Bansal

Last Updated: July 24, 2026

</div>
