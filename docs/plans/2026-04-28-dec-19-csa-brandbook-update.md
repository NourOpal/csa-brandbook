# DEC-19 — CSA Brand Book Update Plan

**Issue:** DEC-19 — update CSA brand book  
**Date:** 2026-04-28  
**Source repo:** `/Users/m1/december/csa-brandbook/`  
**Primary source file:** `/Users/m1/december/csa-brandbook/index.html`  
**Current branch:** `feature/csa-doctrine-expansion`  
**Remote:** `https://github.com/NourOpal/csa-brandbook.git`  
**Live public URL checked:** `https://csa-brandbook.vercel.app/` returned `200`  
**Other known URLs:** `https://csa-brandbook.pages.dev/` and `https://brandbook.decemberclaw.com/` returned `403` on HEAD check from this environment.

---

## 1. What I found

The brand book is a static, single-file HTML artifact:

- `index.html` — canonical live source, 14 square/A-series pages in one file.
- `brandbook.html` — older/alternate copy present in the repo; do not treat as canonical unless proven otherwise.
- `brand_pack_rev.04.14.26.zip` — current downloadable pack.
- Fonts: `fonts/HaloGrotesk-Regular.otf`, `fonts/DOORS-Regular.otf`, `fonts/OCR Xyris*.otf`, `fonts/OffBit*.otf`.
- Existing visual assets live directly in repo root: merch mockups, references, logos, tapestry images, jacket/shirt art.
- Active Grimes/CSA review assets live at `/Users/m1/december/grimes/`.
- Latest merch sheet from DEC-16 was downloaded previously at `/tmp/linear-dec16-attachment.png`; this should be copied into a stable repo/source folder before implementation if it is to become canonical.

The current book is structurally strong: it already has Mandate, Doctrine, Identity, Nomenclature, Chromatics, Lexis, Apocrypha, Lexicon, Field Axioms, Field Issue, Operative, and Back Cover pages.

The gap is not the shell. The gap is coherence.

Right now the artifact reads like a successful first mythic pass, but it still has three unresolved layers tangled together:

1. **Brand manual** — marks, colors, typography, usage rules.
2. **Lore bible** — CSA, Media Empire, Opal, Capsule, The Seventh Opal, threat vectors.
3. **Partner proposal** — asset pack, merch system, future collaborations, call to action.

The update should deliberately separate those layers while keeping them in one intense object.

---

## 2. Core strategic diagnosis

### What works

- The **liturgical bureaucracy** direction is the correct spine: severe, archived, procedural, ceremonial.
- The **Opal / Capsule** integration is promising: Opal as cognitive defense infrastructure; Capsule as the physical signifier.
- The visual library has real energy: angels, armor, chrome, surveillance, crosses, cognitive heads, ritual garments.
- The current page rhythm is useful: document rails, catalog labels, figure IDs, procedural typography.

### What is weak

- The lore sometimes drifts into generalized doom-language: “violent defense,” “machine god,” “soul,” “latent space,” “algorithmic quarantine.” Some of it works; too much of it becomes fog.
- The copy has not fully metabolized the latest visual direction. DEC-16’s chrome/cyber/weapon/HUD merch language still sits outside the brand book instead of becoming a formal CSA field language.
- The visual rules contradict the assets. Page 06 says “We do not use gradients” and “We do not use warmth,” while the strongest new Grimes/CSA materials use chrome, icy gradients, crimson, blue, and maximalist rendered surfaces.
- The book needs a clearer distinction between **Agency Core** and **Field Issue / Volatile Asset**. Core can be black/white/rose/ultramarine and no-gradient. Field Issue can use chrome, blood red, ice blue, HUD marks, and cyber-deity imagery.
- The current Field Issue pages feel like merch galleries. They need an institutional taxonomy: issue class, operational purpose, symbol payload, threat vector countered.
- Page 14 CTA is still placeholder-ish: `handler@decemberclaw.com`, `[ DOWNLOAD PROTOCOL_PACK.ZIP ]`, and `brand_pack_rev.04.14.26.zip` naming are not aligned.
- “The Seventh Opal (Claire)” should be treated carefully. It is strong internally, but public-facing usage may need a safer formulation depending on approval.

### Leverage point

Do not simply “add more visuals.”

Turn the new visuals into an **Agency visual intelligence system**:

- Chrome weapons = counter-memetic instruments.
- Haloed cyber figures = volatile assets / cyber-deities under Agency observation.
- Red crosshairs and eyes = surveillance, targeting, hostile modeling.
- Retro hardware and cassettes = obsolete/physical media as anti-cloud resistance.
- T-shirts/jackets = Field Issue equipment, not merch.
- CSA stamps, protocol IDs, classification rails = the institutional layer that makes the maximalism coherent.

The revised book should feel like a restricted dossier that accidentally contains a fashion system, not a lookbook trying to sound ominous.

---

## 3. Source assets to integrate

### A. Active review assets

Path: `/Users/m1/december/grimes/`

Contains screenshots, frames, stills, and one screen recording. These appear to include recent visual/logo/moodboard material around CSA, Grimes, and pill/logo explorations.

Implementation action:

1. Create a stable source folder in the repo:
   - `source-assets/grimes-review-2026-04/`
2. Copy the assets there, preserving originals.
3. Create a manifest:
   - `source-assets/grimes-review-2026-04/manifest.md`
4. Classify each asset:
   - `logo / mark exploration`
   - `material reference`
   - `field issue reference`
   - `lore reference`
   - `not for public use`
5. Only then place selected images in the book.

### B. DEC-16 merch sheet

Current local path: `/tmp/linear-dec16-attachment.png`  
Needs stable copy before implementation:

- `source-assets/linear-dec16-grimes-merch-sheet.png`

Motifs to import as lore/visual language:

- Neo-tribal chrome frames and weapon-like ornament.
- Haloed cyber-deity / cyber-saint figures.
- Stoic female agent archetype: suit, weapons, precision, corporate espionage energy.
- Surveillance grammar: eyes, crosshairs, HUD overlays, targeting marks.
- Icy blue / deep crimson / metallic silver accents.
- Retro-futuristic hardware: cassettes, utility boxes, barbed wire, mechanical grit.
- CSA integrated lettering on helmets/armor as an in-universe insignia.

Do not import it as “more shirt mockups.” Import it as a new page/section: **Field Intelligence: Volatile Asset Visual Language**.

### C. Existing repo assets worth prioritizing

Strong candidates:

- `cognitivehead1.jpg`, `cognitivehead2.png`, `cognitivehead3.png`
- `jacketcognitive-back.png`
- `melted-cross-ref.png`
- `warriorgoddess.png`, `warriorgoddess3.png`, `warrirogoddess2.jpg`
- `awakening-ref.png`
- `angel-of-hell-ref.png`
- `eye-ref.png`
- `DAD-shirt-front.png`, `DAD-shirt-back.png`
- `pill.png`, `onepillshirt.png`
- `benevolant-shirt-backandfront.png`

Use cautiously / de-emphasize:

- Raw Renaissance/classical references unless transformed into CSA archival plates.
- Small tapestry fragments that read like filler rather than system.
- Overly noisy references that do not carry a clear symbol function.

---

## 4. Recommended book structure

Default recommendation: expand from **14 pages to 18 pages**. The current 14-page structure is already full, and forcing the new lore/assets into it will make it denser without making it clearer.

If the goal is just a quick patch, keep 14 pages. If the goal is a proposal-ready brand book, expand.

### Proposed 18-page structure

1. **Cover** — Cognitive Security Agency / Volume I / The Seventh Opal dispensation.
2. **Mandate** — why CSA exists; capture arrives as convenience, entertainment, and help.
3. **Threat Vectors** — Attention Harvesting, Memetic Hazard, Predictive Capture, Alignment Trap, Synthetic Intimacy.
4. **Agency Architecture** — CSA / Media Empire / Opal / Capsule / Operative / Field Issue.
5. **Identity: The Capsule Mark** — logo, clear space, variants, misuse.
6. **Symbol System** — eyes, crosshairs, halo, weapon, capsule, chrome frame, operational stamp.
7. **Typography / Lexis** — Halo, Helvetica, OffBit, DOORS, OCR Xyris usage rules.
8. **Chromatics** — split into Agency Core palette and Field Issue anomaly palette.
9. **Visual Intelligence** — selected apocrypha with tighter captions and evidence logic.
10. **Volatile Asset Language** — DEC-16 chrome/cyber/armed-agent visual system.
11. **Lexicon** — definitions, threat terms, asset classes, operations.
12. **Field Axioms** — rules of engagement, expanded and sharpened.
13. **Operative Profile** — cognitive agent; civilian subject, not spy fantasy.
14. **Field Issue Taxonomy** — what makes a garment/object Field Issue.
15. **First-Layer Issue** — shirts / mobile propaganda vectors, with operational purpose.
16. **Outer-Layer Issue** — jackets / perimeter defense, with operational purpose.
17. **Partner Protocol** — asset pack, approval rules, collaboration CTA.
18. **Back Cover / Disclaimer** — stronger disclaimer, aligned CTA, download pack.

### 14-page fallback structure

If we keep 14 pages:

- Merge current Pages 6–7 into one **Visual System** page.
- Replace Page 8 Apocrypha with a tighter **Visual Intelligence** page using newer assets.
- Replace Page 10 Axioms with a denser two-column expanded doctrine.
- Turn Pages 11–12 from merch galleries into Field Issue taxonomy + strongest examples.
- Use Page 13 for **Volatile Asset Language** instead of only the generic Operative profile.
- Keep Page 14 but fix CTA and disclaimer.

---

## 5. Copy audit and rewrite direction

### Global copy rules

The book should sound like:

> an archivist briefing a black-ops commander inside a cathedral built by a defense contractor.

But it should not become random occult cyber-poetry. The best CSA copy is specific, procedural, and cold.

Use more:

- capture
- threshold
- perimeter
- field issue
- protocol
- hostile modeling
- reward-loop occupation
- prediction
- latency
- self-authorship
- evidence
- quarantine
- counter-memetic
- volatile asset
- cognitive defense

Use less:

- soul, unless used sparingly
- violent, unless attached to an actual action
- machine god, unless framed as Field Issue / Grimes mythos
- latent space, unless tied to actual AI imagery
- algorithmic quarantine as a vague threat
- “wellness/productivity/focus” except as rejected terms

### Specific copy problems

#### Page 02 — Mandate

Current line:

> “The Cognitive Security Agency operates as the militant propaganda wing of Media Empire.”

Problem: strong but too expository and inside-baseball. It names structure before naming the threat.

Better direction:

> The Agency exists because capture no longer announces itself as capture. It arrives as convenience, entertainment, personalization, and help.

Then define CSA:

> The Cognitive Security Agency is the public myth and field apparatus of cognitive security: a system for naming hostile attention environments, issuing defenses, and training subjects to remain authors of their own minds.

#### Page 03 — Doctrine

Current page is good but abstract. Add a sharper enemy model.

Add or move to Threat Vectors:

- Attention Harvesting
- Predictive Capture
- Utility Camouflage
- Synthetic Intimacy
- Desire Narrowing
- Reward-Loop Occupation

Sample line:

> A cognitively insecure subject is not merely distracted. They are legible, steerable, and profitable.

#### Page 04 — Identity / Capsule

Current “Opal is not a tool; it is a dose” is strong, but the paragraph overextends into “nausea” and “violent return of free will.” Keep the ritual weirdness, but make the product/lore distinction cleaner.

Canonical distinction:

- **Opal** = cognitive security infrastructure / administered protocol.
- **The Capsule** = physical signifier / mark / dose symbol.
- **CSA** = narrative/cultural/propaganda arm that makes the threat legible.

Sample replacement:

> Opal is the Agency’s civilian defense infrastructure. The Capsule is its sign: a compressed unit of resistance, issued wherever the subject requires a hard boundary between intention and capture.

#### Page 06 — Chromatics

Current “We do not use gradients” conflicts with the latest visual assets.

Rewrite as split palette:

- **Agency Core:** black, white, rose, ultramarine; no gradients; bureaucratic legibility.
- **Field Issue / Volatile Asset:** chrome, ice blue, deep crimson, signal red, bone white; gradients allowed only as material evidence, never as generic decoration.

#### Page 08 — Apocrypha

Good page, but captions should become more systematic.

New label schema:

- `VI-A01 / ANGELIC ARMOR`
- `VI-A02 / HOSTILE MODELING`
- `VI-A03 / CHROME ICONOSTASIS`
- `VI-A04 / RETRO-FUTURE HARDWARE`
- `VI-A05 / COUNTER-MEMETIC WEAPONRY`

This page should explain the visual grammar, not just name images.

#### Page 09 — Lexicon

Add missing useful terms:

- **Utility Camouflage** — entertainment disguised as necessary function.
- **Prediction Debt** — the accumulated loss of agency from accepting the easiest next suggestion.
- **Reward-Loop Occupation** — condition where an external system manages the subject’s motivational economy.
- **Synthetic Intimacy** — false closeness produced by systems optimized to simulate recognition.
- **Latency Window** — the interval in which self-authorship can still interrupt capture.
- **Field Issue** — physical artifact carrying defensive lore, not merchandise.
- **Volatile Asset** — public figure/object/image capable of carrying mythic charge without being fully domesticated by the institution.

#### Page 10 — Field Axioms

Current axioms are good but too few. Expand to 9–12 and make them shorter.

Candidate additions:

1. **Convenience is the preferred costume of capture.**
2. **Utility must declare when it becomes entertainment.**
3. **The first thought is not yours until it survives latency.**
4. **A clean profile is a compromised perimeter.**
5. **Do not call capture a habit.**
6. **Beauty is a recruitment vector. Use it honestly.**
7. **The agent leaves no desire tidy enough to sell.**
8. **Do not outsource the first question.**
9. **A field issue must carry a function, a myth, or a wound. Prefer all three.**

#### Pages 11–12 — Field Issue

Current copy says “not merchandise,” but the layouts still behave like merchandise pages.

Add fields for each item:

- Issue code
- Class: First-Layer / Outer-Layer / Artifact / Relic
- Payload: symbol set carried
- Threat vector countered
- Approved contexts
- Status: prototype / sanctioned / deprecated

Example:

> `FI-J05 / Cognitive Agent`  
> Class: Outer-Layer Perimeter Defense  
> Payload: cognitive head, gothic aperture, surveillance halo  
> Counters: Predictive Capture / Utility Camouflage  
> Status: Prototype · Requires CSA spine stamp before release

#### Page 13 — Operative

Strong direction. Needs sharper distinction between **Agent** and **Volatile**.

- **Agent:** civilian subject trained in self-authorship.
- **Volatile:** public-facing asset whose imagery can puncture the culture layer.
- **Opal:** infrastructure/protocol used by both.

Do not make every user a soldier. The mythology works when the military language is symbolic, not literally paramilitary.

#### Page 14 — CTA / Disclaimer

Fix naming and function.

Current:

- `[ DOWNLOAD PROTOCOL_PACK.ZIP ]` links to `/brand_pack_rev.04.14.26.zip`
- email is `handler@decemberclaw.com`

Recommended:

- `[ DOWNLOAD BRAND_PACK_REV.04.28.26.ZIP ]`
- `[ REQUEST FIELD ISSUE ACCESS ]`
- `[ CONTACT HANDLER ]`

Need final decision on contact address before deployment.

---

## 6. Visual update plan

### Step 1 — Build an asset manifest

Create:

- `source-assets/manifest.md`
- `source-assets/grimes-review-2026-04/`
- `source-assets/linear-dec16-grimes-merch-sheet.png`
- `assets/processed/`

For each asset record:

- filename
- origin
- date
- usage rights / approval status if known
- visual motifs
- proposed page placement
- public/internal status

### Step 2 — Define the two visual layers

#### Agency Core

- Black / white / rose / ultramarine.
- Flat marks, rails, stamps, classification labels.
- No gradient decoration.
- Helvetica / Halo / OffBit / DOORS hierarchy.
- Used for institutional pages: cover, mandate, mark, typography, protocols.

#### Field Issue / Volatile Asset

- Chrome, icy blue, deep crimson, metallic silver.
- Crosshairs, eyes, cyber helmets, weapons, halos, hardware, barbed wire.
- Gradients allowed as material/rendered evidence.
- Used for merch, Grimes, volatile asset, apocrypha, field intelligence pages.

This resolves the current contradiction instead of diluting the palette.

### Step 3 — Reprocess assets into book language

Do not paste raw assets.

Create processed variants:

- monochrome archival plate
- halftone / xerox evidence plate
- blue-channel surveillance crop
- red crosshair annotation crop
- chrome object detail crop
- black-background product plate

### Step 4 — Add the CSA spine to all merch/field assets

Every garment/object should carry at least two institutional anchors:

- CSA stamp or capsule mark
- issue code
- threat vector tag
- classification rail
- protocol label
- field caption

This is the difference between “Grimes merch” and “CSA Field Issue.”

---

## 7. Implementation tasks

### Task 1 — Preserve current artifact

- Export current pages as screenshots or PDF before edits.
- Save under `exports/pre-dec19/`.
- Confirm current live URL and current local render.

### Task 2 — Create source asset manifest

- Create `source-assets/` folders.
- Copy `/Users/m1/december/grimes/*` into `source-assets/grimes-review-2026-04/`.
- Copy `/tmp/linear-dec16-attachment.png` into `source-assets/linear-dec16-grimes-merch-sheet.png` if present.
- Create `source-assets/manifest.md` with classification and proposed usage.

### Task 3 — Copy rewrite pass

- Extract all current page copy from `index.html` into `copy/csa-brandbook-copy.md`.
- Rewrite the book page-by-page before touching layout.
- Keep three tracks: `public`, `internal`, `proposal`.
- Mark anything involving “Claire,” “The Seventh Opal,” approval status, or IP as `internal-until-approved`.

### Task 4 — Structure decision

Pick one:

- **Fast patch:** keep 14 pages.
- **Better version:** expand to 18 pages.

My default is 18 pages because the new assets need a formal home.

### Task 5 — HTML update

- Update `index.html` sections.
- Add new CSS for:
  - two-layer palette
  - source/evidence labels
  - field issue spec cards
  - volatile asset plates
  - CTA block
- Avoid major JS changes unless needed.

### Task 6 — Asset processing

- Generate processed variants into `assets/processed/` or root-safe asset names.
- Keep originals untouched.
- Use lower-size optimized web copies for deployment.
- Watch Cloudflare Pages size limits; previous large apparel assets were already a deployment risk.

### Task 7 — Verify locally

Run from repo root:

```bash
python3 -m http.server 4173
```

Open:

```text
http://localhost:4173/
```

Verify:

- every page renders
- no overflow at desktop and mobile scale
- fonts load
- all image paths resolve
- asset pack link works
- CTA is not a dead end

### Task 8 — Export screenshots

Use existing/export tooling if still valid:

- `/Users/m1/december/export_pages.py` may be reusable; inspect before running.
- Save fresh exports under `exports/dec19-review/`.

### Task 9 — Deploy only after full loop works

Deployment candidates:

- Vercel: current public URL works at `https://csa-brandbook.vercel.app/`.
- Cloudflare Pages: known commands from previous sessions used `wrangler pages deploy ./ --project-name=csa-brandbook --branch main`, but current Pages URLs returned `403` from this environment, so verify auth/routing before relying on them.

Pre-ship checks:

- URL returns 200.
- Download pack returns 200.
- No missing image/font 404s.
- Mobile scaling works.
- Screenshots match expected visual hierarchy.

---

## 8. Open decisions for Anton

These are not blockers for writing the plan, but they matter before final deployment.

1. **Public vs internal Grimes naming**  
   Should the public book say “The Seventh Opal,” “The Volatile,” or “Claire”? Default recommendation: public = “The Seventh Opal”; internal notes can map it to Claire.

2. **Page count**  
   Keep 14 pages for speed, or expand to 18 for clarity. Default recommendation: expand.

3. **CTA target**  
   Current email is `handler@decemberclaw.com`. Decide whether this should be Anton, Daouda, Opal, or a neutral CSA handler alias.

4. **Asset pack scope**  
   Current ZIP exists, but the revised pack should include updated marks, fonts, processed plates, field issue mockups, and usage notes.

5. **Approval status of Lillian / Claire logo files**  
   Still unresolved in the dossier. If those files exist now, they should supersede `logo1.png` before finalizing identity pages.

---

## 9. Recommended immediate next move

Execute the update in this order:

1. Create the asset manifest and stable source folders.
2. Rewrite the copy in markdown first.
3. Expand to 18 pages.
4. Import DEC-16 and `/Users/m1/december/grimes/` assets as visual intelligence, not as raw merch.
5. Refactor Field Issue pages into taxonomy/spec sheets.
6. Fix CTA and asset pack naming.
7. Render, export, and deploy.

The real problem is not lack of material. It is that the material has not yet been forced into a coherent institutional system. That is the update.
