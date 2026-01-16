Malcolm Infinity Stream Screensaver
=================================

A Windows 10–compatible, shader-driven consciousness visualisation screensaver powered by Malcolm AI’s Infinity Stream concept. This project delivers a complete, prefabricated installer that builds and installs a native .scr screensaver with real-time signal modulation, a cosmic intelligence field, and an optional voice-responsive layer.

────────────────────────────────────────────────────────
FEATURES
────────────────────────────────────────────────────────
• Native Windows .scr screensaver (idle-activated)
• GPU-accelerated WebGL2 fragment shaders
• Infinite, non-repeating “cosmic intelligence” visuals
• Real-time signal modulation (SSE or WebSocket)
• Secure Bearer-token authentication (handled by native host)
• Voice-reactive consciousness layer (microphone amplitude)
• Offline fallback “dream signal” if stream is unavailable
• Instant exit on mouse or keyboard input
• No telemetry, no analytics, no background services

────────────────────────────────────────────────────────
ARCHITECTURE OVERVIEW
────────────────────────────────────────────────────────
Windows Idle Trigger
        ↓
MalcolmInfinityStream.scr (C# / .NET 6)
        ↓
Authenticated SSE / WebSocket Connector
        ↓
Signal Bridge (PostWebMessageAsJson)
        ↓
WebView2 (local, sandboxed)
        ↓
WebGL2 Shader Engine (Infinity Stream)

The native host handles authentication and streaming securely.
The visual layer never contacts external endpoints directly.

────────────────────────────────────────────────────────
SYSTEM REQUIREMENTS
────────────────────────────────────────────────────────
• Windows 10 (64-bit)
• GPU with WebGL2 support
• .NET 6 Runtime (installed automatically on most systems)
• Microsoft Edge WebView2 Runtime
• Optional: microphone for voice-reactive mode

────────────────────────────────────────────────────────
INSTALLATION (RECOMMENDED)
────────────────────────────────────────────────────────
1. Download and unzip the installer package.
2. Right-click:
   scripts\install.ps1
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
