# Grass Desktop Autologin  
### Fully automated Grass Desktop container with patched xdotool

This project provides a **fully working, reproducible autologin system** for the Grass Desktop application.  
It fixes the upstream xdotool issues, adds environment‑based credential injection, and automates the entire login flow inside a Docker container.

This is the **first fully functional autologin solution** for Grass Desktop.

---

## ✨ Features

- � Automatic login using email + password  
- ⌨️ Patched xdotool typing (fixes `@`, `.`, `!`, etc.)  
- � Reliable Grass window detection  
- � Automated login sequence  
- � Auto‑update toggle automation  
- � Persistent configuration flag (`~/.grass-configured`)  
- � Reproducible Docker build  
- �️ Works headless via VNC / noVNC  
- ⚙️ Environment‑driven configuration  

---

## � Quick Start

Clone the repo:
git clone https://github.com/Sampsonfarms0/grass-desktop-autologin cd grass-desktop-autologin

Copy the example environment file:
cp .env.example .env

Edit your credentials:
nano .env

Build and run:
docker compose build docker compose up -d

Watch logs:
docker logs -f grass-desktop


---

## � File Overview

| File | Purpose |
|------|---------|
| `Dockerfile` | Builds the patched Grass Desktop container |
| `docker-compose.yml` | Runs the container with VNC + environment variables |
| `grass-desktop_main.py` | Fully patched autologin script |
| `.env.example` | Safe template for user credentials |
| `.env` | Your actual credentials (not committed) |

---

## � Support Development

If this project helps you or earns you money, consider supporting development:

BTC:  
ETH:  
XMR:  
BuyMeACoffee:  
Ko‑fi:  

---

## ❤️ Credits

- Original Grass Desktop container by **mrcolorrain**  
- Autologin patching, containerization, and reproducible build by **Sampsonfarms0**  
