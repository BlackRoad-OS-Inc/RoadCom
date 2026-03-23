# RoadCom

> Road Fleet: RoadCom — Internet Computer — self-hostable desktop OS. PROPRIETARY BlackRoad OS integration.

Part of the [BlackRoad OS](https://blackroad.io) ecosystem — [BlackRoad-OS-Inc](https://github.com/BlackRoad-OS-Inc)

---

<h3 align="center"><img width="80" alt="Puter.com, The Personal Cloud Computer: All your files, apps, and games in one place accessible from anywhere at any time." src="https://assets.puter.site/puter-logo.png"></h3>

<h3 align="center">The Internet OS! Free, Open-Source, and Self-Hostable.</h3>

<p align="center">
    <a href="https://puter.com/?ref=github.com"><strong>« LIVE DEMO »</strong></a>
    <br />
    <br />
    <a href="https://puter.com/?ref=github.com">Puter.com</a>
    ·
    <a href="https://puter.com/app/app-center">App Store</a>
    ·
    <a href="https://developer.puter.com" target="_blank">Developers</a>
    ·
    <a href="https://github.com/heyputer/puter-cli" target="_blank">CLI</a>
    ·
    <a href="https://discord.com/invite/PQcx7Teh8u">Discord</a>
    ·
    <a href="https://reddit.com/r/puter">Reddit</a>
    ·
    <a href="https://twitter.com/HeyPuter">X</a>
</p>

<h3 align="center"><img width="800" style="border-radius:5px;" alt="screenshot" src="https://assets.puter.site/puter.com-screenshot-3.webp"></h3>

<br/>

## Puter

Puter is an advanced, open-source internet operating system designed to be feature-rich, fast, and highly extensible. Puter can be used as:

- A privacy-first personal cloud to keep all your files, apps, and games in one secure place, accessible from anywhere at any time.
- A platform for building and publishing websites, web apps, and games.
- An alternative to Dropbox, Google Drive, OneDrive, etc. with a fresh interface and powerful features.
- A remote desktop environment for servers and workstations.
- A friendly, open-source project and community to learn about web development, cloud computing, distributed systems, and much more!

<br/>

## Getting Started

### to install npm and node 

[install](install.md)

### 💻 Local Development

```bash
git clone https://github.com/HeyPuter/puter
cd puter
npm install
npm start
```
**→** This should launch Puter at 
<font color="red"> http://puter.localhost:4100 (or the next available port). </font>



If this does not work, see [First Run Issues](./doc/self-hosters/first-run-issues.md) for
troubleshooting steps.

<br/>

### 🐳 Docker

```bash
mkdir puter && cd puter && mkdir -p puter/config puter/data && sudo chown -R 1000:1000 puter && docker run --rm -p 4100:4100 -v `pwd`/puter/config:/etc/puter -v `pwd`/puter/data:/var/puter  ghcr.io/heyputer/puter
```
**→** This should launch Puter at 
<font color="red"> http://puter.localhost:4100 (or the next available port). </font>

<br/>

### 🐙 Docker Compose

#### Linux/macOS

```bash
mkdir -p puter/config puter/data
sudo chown -R 1000:1000 puter
wget https://raw.githubusercontent.com/HeyPuter/puter/main/docker-compose.yml
docker compose up
```
**→** This should be available at 
<font color="red"> http://puter.localhost:4100 (or the next available port). </font>

<br/>

#### Windows

```powershell
mkdir -p puter
cd puter
New-Item -Path "puter