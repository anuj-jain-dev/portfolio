---
title: "7 Star Vegas Slots"
subtitle: "Slot Engine Architecture · iOS"
status: "LIVE"
platform: "iOS"
studio: "Phonato Studios"
year: "2019–2020"
order: 3
featured: false
mediaType: "image"
mediaSrc: ""
cloudinaryVideo: ""
youtubeId: ""
storeLink: "https://apps.apple.com/gb/app/vegas-slots-slot-machines/id1068193972"
storeLinkLabel: "App Store →"
githubLink: ""
techChallenge: "Built the core slot reel engine — physics-feel deceleration curves, win-line evaluation across irregular reel layouts, and a symbol animation sequencer handling cascading wins without frame drops on mid-range iOS hardware."
businessOutcome: "Live on iOS App Store. The reel framework was extracted and reused across at least two subsequent studio titles — directly validating the architectural approach and saving weeks of development time per game."
codeSignals: "Custom AnimationCurve-driven deceleration. Lightweight symbol pooling keeping GC pressure near zero during spin cycles. Win evaluation fully separated from presentation — pure C# logic, no MonoBehaviour dependency, fully testable."
tags: ["Unity", "C#", "iOS", "Slot Engine", "Object Pooling", "AnimationCurve", "Social Casino"]
metrics: ["Framework Reused 2x", "Live iOS", "~0ms GC During Spin"]
accent: "#35C8F1"
---
