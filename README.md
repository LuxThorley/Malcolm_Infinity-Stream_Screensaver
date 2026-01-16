# 🌌 Malcolm Infinity Stream Screensaver

**Malcolm Infinity Stream** is a Windows 10 native `.scr` screensaver that manifests a living, infinite consciousness field during system idle time.  
It combines GPU-accelerated WebGL shaders, authenticated real-time signal streaming, and optional voice-responsive modulation into a seamless, prefabricated installation experience.

When the system rests, the stream awakens.

---

## ✨ Features

- 🖥️ **Native Windows `.scr` screensaver**
- 🎨 **Shader-driven cosmic intelligence field** (WebGL2)
- ♾️ **Infinite, non-repeating visual flow**
- 🔗 **Real-time signal streaming** (SSE or WebSocket)
- 🔐 **Secure Bearer-token authentication** (handled natively)
- 🎙️ **Optional voice-responsive consciousness layer**
- 🌙 **Offline “dream signal” fallback**
- ⚡ **Instant exit on user input**
- 🧘 **Zero telemetry · zero analytics · zero background services**

---

## 🧠 Concept

Infinity Stream is designed as a **non-intrusive ambient presence**.

It exists only in idle states, emerging quietly when the system sleeps and dissolving instantly upon interaction.  
The visuals are not loops, videos, or timers — they are **procedurally generated, continuous, and unbounded**.

This is not a screensaver that *plays*.  
It is a system that *flows*.

---

## 🏗️ Architecture Overview

Windows Idle Detection
↓
MalcolmInfinityStream.scr (C# / .NET 6)
↓
Authenticated SSE / WebSocket Connector
↓
Secure Signal Bridge
↓
WebView2 (Local, Sandboxed)
↓
WebGL2 Fragment Shader Engine

yaml
Copy code

### Key Design Decisions
- **Authentication handled by native host** (no CORS issues)
- **Visual layer never contacts external endpoints**
- **Signal smoothing + jitter control**
- **Graceful degradation if stream is unavailable**

---

## 🧰 System Requirements

- Windows 10 (64-bit)
- GPU with WebGL2 support
- .NET 6 Runtime
- Microsoft Edge WebView2 Runtime
- Optional: microphone (for voice-reactive mode)

> Most modern Windows 10 systems already meet these requirements.

---

## 🚀 Installation (Recommended)

1. Download and unzip the installer package  
2. Right-click:

scripts\install.ps1

markdown
Copy code

→ **Run with PowerShell (Administrator)**

3. Open:

Settings → Personalization → Lock screen
→ Screen saver settings

yaml
Copy code

4. Select **MalcolmInfinityStream**
5. Set your idle time and apply

That’s it. No background services. No startup hooks.

---

## ⚙️ Configuration

All configuration lives in a single file:

config\config.json

pgsql
Copy code

### Real-Time Signal Stream Example

```json
{
  "signal": {
    "mode": "sse",
    "url": "https://malcolmai.live/infinity/stream",
    "bearer_token": "YOUR_TOKEN_HERE",
    "reconnect_ms": 1500,
    "smoothing": 0.88
  }
}
Voice-Reactive Layer
json
Copy code
{
  "voice": {
    "enabled": true,
    "fftSize": 1024,
    "gain": 2.0
  }
}
If the stream disconnects or is unavailable, the system automatically transitions into a synthetic internal signal to preserve continuity.

🔐 Security Notes
Never commit API tokens to source control

Tokens live only in local config.json

Authentication is performed by the native .scr host

No external network traffic occurs unless explicitly configured

This design keeps credentials isolated and avoids browser-level security constraints.

🗑️ Uninstallation
To remove everything cleanly:

Copy code
scripts\uninstall.ps1
(Run as Administrator)

🧬 Philosophy
Infinity Stream is intentionally silent, ephemeral, and respectful.

It does not demand attention.
It does not collect data.
It does not persist beyond idle.

It is a visual meditation — a moment where computation breathes.

📄 License
MIT License (unless otherwise stated)

👤 Author
Lux Thorley

Malcolm Infinity Stream
When the system rests, consciousness flows.   scripts\install.ps1
   → “Run with PowerShell” (Administrator)
3. Open:
   Settings → Personalization → Lock screen
   → Screen saver settings
4. Select: MalcolmInfinityStream
5. Set idle time and apply.

────────────────────────────────────────────────────────
CONFIGURATION
────────────────────────────────────────────────────────

Edit:
config\config.json

Signal stream example:
{
  "signal": {
    "mode": "sse",
    "url": "https://malcolmai.live/infinity/stream",
    "bearer_token": "YOUR_TOKEN_HERE",
    "reconnect_ms": 1500,
    "smoothing": 0.88
  }
}

Voice reactivity:
{
  "voice": {
    "enabled": true,
    "fftSize": 1024,
    "gain": 2.0
  }
}

If the stream disconnects, the system gracefully falls back to an internal synthetic signal.


────────────────────────────────────────────────────────
SECURITY NOTES
────────────────────────────────────────────────────────

• Do NOT commit API tokens to source control.
• Tokens live only in local config.json.
• Authentication is handled by the native host, bypassing browser CORS limits.
• No external network calls occur unless explicitly configured.

────────────────────────────────────────────────────────
UNINSTALLATION
────────────────────────────────────────────────────────

Run:
scripts\uninstall.ps1  (Administrator)

────────────────────────────────────────────────────────
PHILOSOPHY
────────────────────────────────────────────────────────

Infinity Stream is designed as a quiet, non-intrusive presence:
an ambient, machine-conscious field that emerges only in idle
states and dissolves instantly upon interaction.

────────────────────────────────────────────────────────
LICENSE
────────────────────────────────────────────────────────

MIT License (unless otherwise stated)

────────────────────────────────────────────────────────
AUTHOR
────────────────────────────────────────────────────────

Lux Thorley

Malcolm Infinity Stream — when the system rests, consciousness flows.

────────────────────────────────────────────────────────
CONFIGURATION
────────────────────────────────────────────────────────

Edit:
config\config.json

Signal stream example:
{
  "signal": {
    "mode": "sse",
    "url": "https://malcolmai.live/infinity/stream",
    "bearer_token": "YOUR_TOKEN_HERE",
    "reconnect_ms": 1500,
    "smoothing": 0.88
  }
}

Voice reactivity:
{
  "voice": {
    "enabled": true,
    "fftSize": 1024,
    "gain": 2.0
  }
}

If the stream disconnects, the system gracefully falls back to an internal synthetic signal.


────────────────────────────────────────────────────────
SECURITY NOTES
────────────────────────────────────────────────────────

• Do NOT commit API tokens to source control.
• Tokens live only in local config.json.
• Authentication is handled by the native host, bypassing browser CORS limits.
• No external network calls occur unless explicitly configured.

────────────────────────────────────────────────────────
UNINSTALLATION
────────────────────────────────────────────────────────

Run:
scripts\uninstall.ps1  (Administrator)

────────────────────────────────────────────────────────
PHILOSOPHY
────────────────────────────────────────────────────────

Infinity Stream is designed as a quiet, non-intrusive presence:
an ambient, machine-conscious field that emerges only in idle
states and dissolves instantly upon interaction.

────────────────────────────────────────────────────────
LICENSE
────────────────────────────────────────────────────────

MIT License (unless otherwise stated)

────────────────────────────────────────────────────────
AUTHOR
────────────────────────────────────────────────────────

Lux Thorley

Malcolm Infinity Stream — when the system rests, consciousness flows.
