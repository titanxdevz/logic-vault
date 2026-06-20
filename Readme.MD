# Logic Vault

**A growing collection of reverse-engineered, conceptual system architecture breakdowns.**

This repository documents how large-scale, real-time systems are *likely* architected — based on publicly known engineering patterns, protocols, and best practices. Each folder is a self-contained deep-dive into one system: its components, data flow, protocols, and design rationale, paired with diagrams (image + Mermaid).

This is **not** official or leaked source material from any company. It's an educational/research archive built by studying how systems like these are commonly designed in the industry.

---

## How this repo is organized

Each topic lives in its own folder at the root level:

```
logic-vault/
├── README.md                          ← you are here
├── discord-voice-call-logic/
│   ├── README.md
│   └── (diagram assets)
├── <next-topic-folder>/
│   ├── README.md
│   └── (diagram assets)
└── ...
```

**Convention for every folder:**
- Folder name: `kebab-case`, format `<platform>-<feature>-logic` (e.g. `discord-voice-call-logic`, `spotify-streaming-logic`)
- Must contain its own `README.md` with: Overview → Layered breakdown → Tables → Mermaid diagrams → Glossary → Credits/Disclaimer
- Original schematic/sketch image (if any) included alongside the README, referenced via relative path

---

## Index of Topics

| Folder | Topic | Status |
|---|---|---|
| [`discord-voice-call-logic`](./discord-voice-call-logic/) | Discord real-time voice call & connection architecture (call routing, UDP/WebRTC, SRTP/DTLS, Redis, Kafka) | ✅ Documented |

*(New entries get added here as new folders are added.)*

---

## Why this exists

Most public system design content is either too shallow (high-level blog posts) or doesn't exist at all for closed-source platforms. This repo is an attempt to go deep — tracing a request/data flow end-to-end, documenting protocol choices, tables, and tradeoffs — purely for learning and reference purposes.

## Disclaimer

All content in this repository is conceptual and based on public, general-purpose knowledge of distributed systems, networking protocols, and common industry architecture patterns. None of it represents confirmed, official, or proprietary internal documentation of any company or platform named in these docs.

## License

Feel free to fork, learn from, and contribute. (Add a LICENSE file — MIT recommended — if you want this open for reuse.)
