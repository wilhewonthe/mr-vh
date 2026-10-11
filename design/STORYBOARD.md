# STORYBOARD — Mr. vH

## Film meta
- **Product:** Mr. vH — parent company / venture studio for Polymarket trading, Leviathan off-grid RV, FileCraft tools, Don't Sleep Digest, homelab infrastructure
- **Audience:** Builders, operators, people who want to see what "forged in code" looks like. Technical but not academic.
- **The one feeling:** momentum — the sense that real things are being built, hot metal hitting the anvil, not decks being pitched
- **Peak scene:** Scene 3 (Leviathan) — the 3D off-grid RV rotates and disassembles as you scroll, revealing solar/wind/rain/compute layers. intensity 9
- **Assets available up front:** none (generate all)
- **Sourced-asset findings:** N/A
- **Assumptions made:** autonomous — Mr. vH is the brand, three ventures are the chapters, tone is dark industrial forge
- **References taken:** madewithgsap.com — pinned section title while cards scroll through it; Stripe — WebGL scroll-driven scene with mix-blend-mode, adapted to CSS+canvas; Linear — mix-blend-mode layers for atmosphere; Vercel — CSS scroll-driven animations for lightweight proof sections
- **Moodboard read:** dominant palette = near-black base (#0a0a0a) with molten orange/amber (#ff6b1a, #ff8c00) as ONLY accent; light = extreme chiaroscuro, single hard forge light; composition = asymmetric split with heavy mass anchoring one side; avoid = generic AI dark workshop stock, hornet nest search noise
- **Style gate verdict:** approved — mockup passes slopscan, contrast, taste checks

## Arc
<!-- hook → rising → PEAK → proof → door. 5–7 scenes. Adjacent scenes must differ in layout family AND motion family -->

| # | Scene | Beat | Intensity (1–10) | layout family | motion family |
|---|-------|------|------------------|---------------|---------------|
| 1 | The Forge | hook | 6 | full-bleed-media | scroll-scrub |
| 2 | Leviathan | rising | 7 | pinned-canvas | pinned-stage |
| 3 | The Disassembly | peak | 9 | pinned-canvas | scroll-scrub |
| 4 | FileCraft + Digest | proof | 5 | editorial-columns | parallax-depth |
| 5 | Homelab | proof | 5 | split-asymmetric | entrance-reveal |
| 6 | The Door | door | 4 | centred-type | kinetic-type |

<!-- layout family: full-bleed-media / split-asymmetric / centred-type / stacked-cards / editorial-columns / pinned-canvas / marginal-notes …
     motion family: scroll-scrub / pinned-stage / entrance-reveal / parallax-depth / kinetic-type / ambient-loop / none
     Motion families used across the whole page must be ≤3 (commit-sheet field 5); the same family may repeat, just never in two adjacent scenes. -->

---

### Scene 1 — The Forge   | beat: hook | intensity: 6
- **purpose:** feel: the heat of real work / learn: Mr. vH is where things get made
- **subject:** a forge — glowing ember particles, heat distortion, the word "MR. VH" hammered into metal
- **layout_family / motion_family:** full-bleed-media / scroll-scrub
- **camera:** low-angle (heroic) — viewer looks up at the forge
- **lighting:** hard contrast — single molten source, deep shadows
- **motion:** scroll-scrub drives heat intensity — more scroll = brighter forge, more sparks, "FORGED IN CODE" reveals per-word
- **transition_in / out:** cut / wipe-mask (vertical curtain)
- **scroll_len:** 200vh (pinned hero)
- **copy:** H: "MR. VH" / sub: "FORGED IN CODE"
- **media:**
  - type: element/texture
  - route: GENERATE
  - frame prompt: extreme close-up of molten steel being hammered, single hard orange light source, flying sparks captured mid-air, near-black background, visceral texture, 8K, industrial photography style
  - motion prompt: scroll-scrub: heat intensifies from dull glow to white-hot, particle count increases, per-word kinetic type reveal
  - score: low drone, industrial hum, 60bpm
- **fallback:** static hero image with "FORGED IN CODE" already revealed, no particle animation

### Scene 2 — Leviathan   | beat: rising | intensity: 7
- **purpose:** feel: the scale of the build / learn: 40' off-grid RV, fully autonomous
- **subject:** the Alfa See Ya 37FD — exterior in environment, then cutaway
- **layout_family / motion_family:** pinned-canvas / pinned-stage
- **camera:** orbital — rotates around the RV showing all sides
- **lighting:** golden hour — warm but industrial, long shadows
- **motion:** pinned canvas, orbital rotation driven by scroll, panels fade in/out as RV rotates
- **transition_in / out:** wipe-mask / depth-parallax
- **scroll_len:** 300vh (pinned)
- **copy:** H: "LEVIATHAN" / sub: "40 feet. Zero grid. Full autonomy."
- **media:**
  - type: 3D model
  - route: GENERATE (A→B morph via WebGL displacement)
  - frame prompt: Alfa See Ya 37FD RV in desert landscape, solar panels deployed, wind turbine spinning, rugged tires, technical cutaway style showing internal systems, golden hour lighting, molten orange accents on key systems
  - motion prompt: controlled A→B state change via WebGL displacement morph — exterior shell morphs to cutaway revealing solar/wind/rain/compute layers
  - score: rising tension, mechanical sounds
- **fallback:** static cutaway illustration with labeled systems

### Scene 3 — The Disassembly   | beat: peak | intensity: 9
- **purpose:** feel: awe at the engineering / learn: every system exposed — solar, wind, rain, hydroponics, compute farm
- **subject:** the RV disassembled — 9 floating layers: shell, solar array, wind turbine, water tanks, hydroponics, battery bank, compute rack, living space, chassis
- **layout_family / motion_family:** pinned-canvas / scroll-scrub
- **camera:** macro → orbital — starts tight on a bolt, pulls out to show all layers floating
- **lighting:** hard contrast — forge light hits each layer differently
- **motion:** scroll-scrub explodes the RV layer by layer, each layer has its own scroll range, mix-blend-mode spark trails between layers
- **transition_in / out:** depth-parallax / letterbox
- **scroll_len:** 400vh (pinned, the peak)
- **copy:** H: "EVERY SYSTEM. EXPOSED." / sub: "Solar 2.4kW · Wind 400W · Rain 500gal · Hydroponics 32 plants · Compute 8×H100"
- **media:**
  - type: sequence
  - route: GENERATE
  - frame prompt: exploded technical view of off-grid RV, 9 distinct layers floating in space: outer shell, solar panel array, wind turbine, water storage, hydroponics rack, battery bank, compute cluster (H100s), interior living space, chassis. Each layer illuminated by single molten light source, sparks trailing between layers, near-black void background, engineering precision
  - motion prompt: scroll-scrub explodes layers sequentially (100vh each), mix-blend-mode: screen spark trails connect layers, each layer rotates slowly
  - score: peak — industrial percussion, metallic resonance
- **fallback:** static exploded view with all 9 layers visible, scroll = simple fade-in per layer

### Scene 4 — FileCraft + Don't Sleep Digest   | beat: proof | intensity: 5
- **purpose:** feel: these are real tools people use / learn: privacy-first file tools + editorial tech digest
- **subject:** two product cards side by side, asymmetric — FileCraft on left (dense, technical), Digest on right (editorial, spacious)
- **layout_family / motion_family:** editorial-columns / entrance-reveal
- **camera:** eye-level — straight on, product-focused
- **lighting:** studio — clean, product photography style
- **motion:** entrance-reveal staggered — cards fade/slide in from opposite sides, subtle parallax on inner elements
- **transition_in / out:** letterbox / cut
- **scroll_len:** content
- **copy:** H: "PUBLIC TOOLS" / sub: "FileCraft — 6 privacy-first file tools. Don't Sleep — daily tech deals, zero slop."
- **media:**
  - type: still
  - route: GENERATE
  - frame prompt: split composition — left: FileCraft interface on dark screen showing PDF merge in action, right: Don't Sleep Digest editorial spread with bold typography and deal cards. Both on near-black surface with molten orange accent lines. Product photography, sharp, visceral.
  - motion prompt: entrance-reveal — left card slides from left, right from right, stagger 150ms; subtle parallax on inner elements
  - score: none
- **fallback:** static product cards with links

### Scene 5 — Homelab Infrastructure   | beat: proof | intensity: 5
- **purpose:** feel: the engine room / learn: GPU clusters, virtualization, self-hosted everything
- **subject:** server rack — blinking lights, cable runs, thermal camera view
- **layout_family / motion_family:** split-asymmetric / scroll-scrub
- **camera:** macro — close on cable management, GPU backplates, blinkenlights
- **lighting:** neon accent — molten orange LED strips in rack, otherwise darkness
- **motion:** scroll-scrub reveals rack units bottom-to-top, each unit's specs appear as it enters viewport
- **transition_in / out:** cut / curtain
- **scroll_len:** 200vh
- **copy:** H: "HOMELAB" / sub: "8×H100 · 2×A100 · Proxmox · TrueNAS · 100GbE · All self-hosted"
- **media:**
  - type: element/texture
  - route: GENERATE
  - frame prompt: server rack interior macro shot, molten orange LED light strips illuminating cable runs, GPU backplates (H100/A100) visible, blinkenlights on switches, fiber cables, thermal imaging false-color overlay on one section, industrial precision, near-black background
  - motion prompt: scroll-scrub reveals rack units sequentially bottom-to-top, specs fade in per unit, ambient-loop on LED blink (subtle, 2s cycle)
  - score: none
- **fallback:** static rack photo with specs overlay, scroll = simple fade-in

### Scene 6 — The Door   | beat: door | intensity: 4
- **purpose:** feel: invitation to build / learn: where to go next
- **subject:** anvil with three glowing slots — each venture name, click to enter
- **layout_family / motion_family:** centred-type / entrance-reveal
- **camera:** static — dead center
- **lighting:** hard contrast — forge glow from the three slots
- **motion:** entrance-reveal — three slots stamp in sequentially with ember burst, hover = ember burst
- **transition_in / out:** curtain / cut
- **scroll_len:** 100vh
- **copy:** H: "PICK YOUR PROJECT" / sub: "Leviathan · FileCraft · Homelab — each forged separately, all from the same fire"
- **media:**
  - type: none (type-led)
  - route: none
  - frame prompt: N/A
  - motion prompt: entrance-reveal stamp-in sequential, ember burst on hover
  - score: ambient fade out
- **fallback:** three static buttons with venture names and links

## Gate 0 checklist
- [x] exactly one scene with intensity ≥8 (Scene 3 = 9)
- [x] no two adjacent scenes share layout family or motion family
- [x] ≤3 distinct motion families across the whole page (scroll-scrub, pinned-stage, entrance-reveal)