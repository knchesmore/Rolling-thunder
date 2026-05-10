# ⚔ TTRPG Dice Roller — Owlbear Rodeo Extension

A dark-fantasy styled dice roller for Owlbear Rodeo with **named preset saves** and one-click rolling.

## Features

- **All standard TTRPG dice**: d2, d4, d6, d8, d10, d12, d20, d100
- **Multi-die rolls**: click the same die multiple times to add more (2d6, 3d8, etc.)
- **Modifier support**: add/subtract a flat modifier to any roll
- **Named presets**: save any combination with a custom name (e.g. "Sneak Attack", "Fireball")
- **One-click preset roll**: click the preset name to instantly roll it
- **Load preset**: load a preset back into the builder to tweak it
- **Roll results**: shows total, individual die results, and highlights max (gold) and min (red) rolls
- **Persistent presets**: saved to localStorage, survive page reloads

---

## Installation in Owlbear Rodeo

### Option A — Host it yourself (recommended)

1. Upload all files (`manifest.json`, `index.html`, `icon.svg`) to any static hosting:
   - [Netlify Drop](https://app.netlify.com/drop) — drag & drop, free, instant URL
   - [GitHub Pages](https://pages.github.com/)
   - [Vercel](https://vercel.com/), [Cloudflare Pages](https://pages.cloudflare.com/), etc.

2. In Owlbear Rodeo, go to **Extensions → Add Extension**

3. Enter your hosted URL (e.g. `https://your-dice-roller.netlify.app`)

4. The extension will appear in your OBR toolbar!

### Option B — Local development (for testing)

1. Install [Node.js](https://nodejs.org/)
2. In the extension folder, run:
   ```bash
   npx serve .
   ```
3. This starts a local server at `http://localhost:3000`
4. In OBR → Extensions → Add Extension → enter `http://localhost:3000`

> **Note**: OBR requires HTTPS for production extensions. Local `http://localhost` works in dev mode.

---

## How to Use

1. **Click dice** to add them to your roll formula
2. **Set a modifier** (positive or negative) if needed
3. **Click Roll the Dice** to roll
4. **Save Preset**: click "+ Save Preset", type a name, click Save
5. **One-click roll**: click any preset name in the list to instantly roll it
6. **Load preset**: click "↑ Load" to bring a preset into the builder for editing

---

## File Structure

```
dice-roller-extension/
├── manifest.json   ← OBR extension manifest
├── index.html     ← The dice roller UI panel
├── icon.svg        ← Extension icon
└── README.md       ← This file
```
