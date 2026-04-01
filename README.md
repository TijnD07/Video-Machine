# 🚀 VideoMachine: Automated Content Engine

Een krachtige, end-to-end automatiseringstunnel ontwikkeld in n8n om het proces van content creatie volledig te automatiseren. Dit project scant, downloadt en rendert Twitch-clips naar kant-en-klare video-content zonder handmatige tussenkomst van een editor.

## 🌟 Belangrijkste Features
- **Twitch Clip Discovery:** Automatische monitoring van specifieke kanalen voor de nieuwste en populairste clips via API-integraties.
- **High-Performance Rendering:** Gebruik van een geïntegreerde FFmpeg-engine voor het schalen, knippen en renderen van video's direct op de server.
- **Slimme Downloader:** Implementatie van `yt-dlp` binnen een Docker-omgeving voor razendsnelle en betrouwbare media-extractie.
- **Modulaire Architectuur:** Efficiënt gebruik van sub-workflows (zoals de 'Clip Renderer') voor een overzichtelijke en schaalbare logic-flow.
- **Error Handling & Logs:** Uitgebreide foutrapportage en automatische retry-logica bij netwerk- of API-onderbrekingen.
- **Cloud-Ready Infrastructure:** Volledig bereikbaar via een beveiligde Nginx Proxy (Websockets) voor real-time monitoring van de workflow-status.

## 🛠️ Tech Stack
- **Orkestratie:** [n8n](https://n8n.io/) (Self-hosted v1.x)
- **Video Processing:** FFmpeg (Command-line toolset)
- **Scraping & Download:** Python 3 & yt-dlp
- **Containerization:** Docker & Portainer (Debian-based images)
- **Infrastructuur:** Proxmox LXC op een dedicated HP node (Server-grade hardware)
- **Networking:** Nginx Proxy Manager (SSL, Websocket tunneling)

## 📈 Impact
De 'VideoMachine' overbrugt de kloof tussen ruwe livestream-data en publiceerbare content op social media. Dit resulteert in:
- **100% Tijdsbesparing:** Geen handmatige downloads of rendering-wachttijden meer voor de gebruiker.
- **Consistente Output:** Altijd een constante stroom aan verse clips beschikbaar voor social media kanalen.
- **Schaalbaarheid:** De architectuur is eenvoudig uit te breiden naar platforms zoals YouTube, TikTok of Instagram.

## 📸 Preview
![n8n Workflow Overview](assets/n8n-workflow-main.png)
![Clip Renderer Sub-flow](assets/n8n-subflow-renderer.png)

---
*Ontwikkeld door Tijn - 2026*
