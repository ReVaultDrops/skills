# Bankr: Frontline — 3D Cyber Tactical Arena

`bankr-frontline` is a browser-first 3D tactical arena shooter built on Three.js and WebRTC PeerJS, adapted from Riposte Frontline.

## Engine Highlights
- **Zero-Server Multiplayer**: WebRTC peer-to-peer lobbies powered by PeerJS.
- **Procedural 3D Geometry**: Low-poly tactical arenas, 50 baked animation clips, 221 prefabs, and dynamic bots without external 3D modeling assets.
- **Web3 / Terminal Native**: Embeddable in Bankr terminal apps with wager duel hooks.

## Deployment Instructions
1. Push the compiled `dist/` directory (containing `riposte-frontline.html`, `sfx/`, `tex/`, and `maps/`) to GitHub Pages or Vercel.
2. In your Bankr App iframe or client, point to the hosted deployment URL.
3. Configure PeerJS lobby rooms for direct community matches.
