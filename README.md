# 🕹️ RetroArcade — Free Retro Gaming on GitHub Pages

A beautiful retro gaming portal you can host **100% free** on GitHub Pages.
Uses **EmulatorJS** (CDN, no install needed) to emulate NES, SNES, GBA, Sega Genesis, and more — right in the browser.

## 🚀 Quick Setup (5 minutes)

### 1. Create a GitHub repository
- Go to **github.com** → click **New** → name it `retro-arcade`
- Set it to **Public**

### 2. Upload these files
Upload all files from this folder to your repo root.

### 3. Enable GitHub Pages
- Go to your repo → **Settings** → **Pages**
- Source: **Deploy from branch** → `main` → `/ (root)` → **Save**
- Your site will be live at: `https://YOUR_USERNAME.github.io/retro-arcade`

---

## 🎮 Adding Games

### Option A: Link to Archive.org (easiest, fully legal)
Archive.org hosts a massive library of classic games with browser emulation built in. Just link to them.

### Option B: Load ROMs locally (user's own files)
The site already supports drag-and-drop ROM loading. Users can drop any ROM file and it plays instantly in their browser. **The file never leaves their computer.**

### Option C: Host your own ROMs (only games you own)
1. Create a `/roms/` folder in your repo
2. Add your ROM files (e.g., `roms/nes/mygame.nes`)
3. In `index.html`, add a card like this:

```html
<div class="game-card" onclick="launchEmulator('roms/nes/mygame.nes', 'nes', 'My Game')">
  <div class="game-thumb-placeholder">🎮</div>
  <div class="game-info">
    <div class="game-title">MY GAME TITLE</div>
    <div class="game-meta">
      <span class="badge badge-console">NES</span>
    </div>
    <div class="play-btn">▶ PLAY NOW</div>
  </div>
</div>
```

---

## 🎯 Supported Systems (EmulatorJS cores)

| System | Core name | File extension |
|--------|-----------|---------------|
| NES | `nes` | `.nes` |
| SNES | `snes` | `.smc`, `.sfc` |
| Game Boy | `gb` | `.gb` |
| Game Boy Color | `gb` | `.gbc` |
| Game Boy Advance | `gba` | `.gba` |
| Sega Genesis | `segaMD` | `.md`, `.bin` |
| Sega Master System | `segaMS` | `.sms` |
| Nintendo 64 | `n64` | `.z64`, `.n64` |
| PlayStation 1 | `psx` | `.bin`, `.iso` |
| Arcade (MAME) | `arcade` | `.zip` |

---

## 🆓 Free & Legal ROM Sources

- **[archive.org/details/NESLibrary](https://archive.org/details/NESLibrary)** — NES games, browser playable
- **[archive.org/details/classicpcgames](https://archive.org/details/classicpcgames)** — classic PC games
- **[itch.io homebrew NES ROMs](https://itch.io/games/tag-nes-rom/tag-free)** — free original NES homebrew games
- **[nesworld.com/homebrew.php](https://www.nesworld.com/homebrew.php)** — freeware NES games
- **[pdroms.de](https://pdroms.de)** — public domain ROMs for many systems

---

## ⚠️ Legal Notice

This site does not host, distribute, or link to copyrighted ROM files. 
Users are responsible for only playing ROMs of games they legally own.
Emulation technology is legal; distributing copyrighted ROMs is not.

---

## 🔧 Tech Stack

- **Pure HTML/CSS/JS** — no build step, no server needed
- **[EmulatorJS](https://emulatorjs.org)** — open source, CDN-hosted
- **GitHub Pages** — free hosting
- **Google Fonts** — Press Start 2P & VT323 for authentic retro feel
