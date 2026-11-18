# Rolagem

Lyrics in playlists with auto-scroll, for playing guitar. Free, no ads, no account.
Built for a friend (2026-11-18).

- Single-file web app (`index.html`) + manifest + service worker → installs on iPhone via
  Safari → Share → "Adicionar à Tela de Início"; works offline after the first load.
- Lyrics: search via [LRCLIB](https://lrclib.net) (open, free, no key) or paste by hand.
- Everything is stored on the phone (localStorage). Backup/restore via ⋯ on the home screen.
- Speed is remembered per song; "Ajustar à duração" fits the scroll to the track length.
- Screen stays awake while scrolling (Wake Lock, iOS 16.4+).

Run locally: `python3 -m http.server 8793` → http://127.0.0.1:8793
Needs HTTPS to install on a phone (e.g. GitHub Pages).
