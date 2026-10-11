# REFERENCES — scouted 2026-10-04

Mechanics, not skins. For each reference name the ONE idea you are taking and how it
changes for this brand. Copying a reference wholesale is slop with better taste.

| # | site | stack detected | page shape | mechanics |
|---|---|---|---|---|
| 1 | [madewithgsap.com](https://madewithgsap.com) | GSAP, ScrollTrigger, ScrollSmoother, SplitText | 22.1× vh, 14 sections | 4 pinned scene(s) (GSAP ScrollTrigger); smoothed/virtualised scroll |
| 2 | [stripe.com](https://stripe.com) | three.js, Framer Motion | 17× vh, 131 sections | WebGL scene driven by scroll; 5 mix-blend-mode layer(s) |
| 3 | [linear.app](https://linear.app) | Framer Motion | 11.1× vh, 103 sections | 16 mix-blend-mode layer(s) |
| 4 | [vercel.com](https://vercel.com) | Framer Motion | 6.2× vh, 12 sections | CSS scroll-driven animations (animation-timeline); 4 mix-blend-mode layer(s) |

## 1. Made With Gsap
- url: https://madewithgsap.com
- stack: GSAP, ScrollTrigger, ScrollSmoother, SplitText, Lenis, Matter.js
- mechanics: 4 pinned scene(s) (GSAP ScrollTrigger); smoothed/virtualised scroll
- page: 22.1× viewport tall · 14 sections · 0 canvas · 4 video
- type: display `LayGrotesk 120px/500` (largest painted text: "freshly added") · body `LayGrotesk` · @font-face: LayGrotesk, PPNeueMontrealMono
- palette (most painted): #0a0a0b ×378 · #ffffff ×364 · #999999 ×57 · #000000 ×51 · #c9fe6e ×8 · #f3f3f3 ×6
- shots: `shots/madewithgsap.com-00.png` `shots/madewithgsap.com-01.png` `shots/madewithgsap.com-02.png`  ← look at the hero; look at the rest only if you take a steal from this one
- **steal:** pinned section title while cards/content scrolls through it; we'll use this for the venture chapters — the venture name stays pinned while its projects scroll past | Financial Infrastructure to Grow Your Revenue
- url: https://stripe.com
- stack: three.js, Framer Motion  ·  built with Next.js
- mechanics: WebGL scene driven by scroll; 5 mix-blend-mode layer(s)
- page: 17× viewport tall · 131 sections · 5 canvas (WebGL live) · 0 video
- type: display `sohne-var, "SF Pro Display", sans-serif 56px/300` (largest painted text: "The backbone of global comme") · body `sohne-var, "SF Pro Display", sans-serif`
- palette (most painted): #000000 ×1608 · #533afd ×790 · #061b31 ×303 · #50617a ×229 · #ffffff ×174 · #64748d ×145
- shots: `shots/stripe.com-00.png` `shots/stripe.com-01.png` `shots/stripe.com-02.png`  ← look at the hero; look at the rest only if you take a steal from this one
- **steal:** WebGL scene driven by scroll with mix-blend-mode layers; we adapt this for the hero — a "forge" that responds to scroll (heat intensifies, sparks fly) but built with CSS + canvas, not three.js

## 3. Linear – The system for product development
- url: https://linear.app
- stack: Framer Motion
- mechanics: 16 mix-blend-mode layer(s)
- page: 11.1× viewport tall · 103 sections · 0 canvas · 0 video
- type: display `"Inter Variable", "SF Pro Display", -apple-system, BlinkMacS 72px/510` (largest painted text: "Built for the future. Availa") · body `"Inter Variable", "SF Pro Display", -apple-system, BlinkMacSystemFont,`
- palette (most painted): #f7f8f8 ×2631 · #8a8f98 ×434 · #62666d ×284 · #d0d6e0 ×199 · #ffffff ×165 · #e2e4e7 ×142
- shots: `shots/linear.app-00.png` `shots/linear.app-01.png` `shots/linear.app-02.png`  ← look at the hero; look at the rest only if you take a steal from this one
- **steal:** heavy use of mix-blend-mode for depth and atmosphere; we'll use mix-blend-mode: screen/overlay for spark/ember layers over the dark base

## 4. Agentic Infrastructure - Vercel
- url: https://vercel.com
- stack: Framer Motion
- mechanics: CSS scroll-driven animations (animation-timeline); 4 mix-blend-mode layer(s)
- page: 6.2× viewport tall · 12 sections · 1 canvas · 0 video
- type: display `GeistSans, "GeistSans Fallback" 64px/400` (largest painted text: "Agentic Infrastructure") · body `GeistSans, "GeistSans Fallback"` · @font-face: Geist Mono, GeistSans, GeistSans Fallback, GeistPixelSquare, GeistPixelGrid, GeistPixelCircle, GeistPixelTriangle, GeistPixelLine
- palette (most painted): #171717 ×866 · #4d4d4d ×209 · #8f8f8f ×30 · #ffffff ×26 · #c9c9c9 (lab(80.976 0 -0.0000119209)) ×12 · #fafafa ×10
- shots: `shots/vercel.com-00.png` `shots/vercel.com-01.png` `shots/vercel.com-02.png`  ← look at the hero; look at the rest only if you take a steal from this one
- **steal:** CSS scroll-driven animations (animation-timeline) for lightweight parallax; we'll use this for the "proof" sections where metrics/reveals happen without heavy JS
