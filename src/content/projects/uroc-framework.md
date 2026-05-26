---
title: Slot Framework @ UROC Studios
subtitle: Scalable Multi-Title Architecture · Remote
status: CURRENT
platform: Multi-title
studio: UROC Studios (Isle of Man)
year: 2024–Present
order: 2
featured: false
mediaItems:
  - type: video
    cloudinaryUrl: https://res.cloudinary.com/dcbzgebuv/video/upload/q_auto/f_auto/v1779785482/Penguin_ijjtkm.mp4
    label: Collect&Rock
  - type: video
    label: HoldForGold
    cloudinaryUrl: https://res.cloudinary.com/dcbzgebuv/video/upload/q_auto/f_auto/v1779790694/medusa_len3tp.mp4
storeLink: ""
storeLinkLabel: ""
githubLink: ""
techChallenge: Rearchitecting a shared slot framework to support divergent game
  configs — reel sizes, bonus mechanics, win presentations — without forking per
  title. Feature-flag system + Spine-driven animations replacing legacy sprite
  sheets.
businessOutcome: Framework powers multiple live titles. Spine migration cut
  artist iteration time significantly. Remote collaboration across time zones
  with async-first PRs and documented architecture decision logs.
codeSignals: "Spine runtime optimisation: shared atlas, runtime skin swapping.
  Unity Timeline (PlayableDirector) for win sequences. Feature-flag architecture
  via ScriptableObjects — mechanics toggled per title without code branching."
tags:
  - Unity
  - C#
  - Spine
  - Unity Timeline
  - ScriptableObject
  - Remote
accent: "#0891b2"
---
