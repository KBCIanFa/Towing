# Towing (and a couple of Aussie-flavoured web tools)

A small collection of **single-file, static HTML** tools you can open in any browser — no build step, no install, no drama.

At the moment the repo includes:
- **Car Selector** (including an “Alpha Release” variant) aimed at Australians, with filters and a section for **caravan/trailer specs** (ATM/GTM/ball weight etc.).  
- **The Grumpy Old Man Course** — a tongue-in-cheek “apprenticeship” page with offline tools, progress tracking, and an optional “Cheeky AI” settings panel.

## What’s in this repo

### 🚗 Car Selector
Files:
- `Car Selector1.html`
- `Car SelectorV2.html` (labelled “Car Selector Alpha Release”)  

What it does (current UI):
- Filters for common vehicle criteria (use-case, body style, drivetrain, seats, cylinders, towing capacity, ANCAP, fuel consumption, fuel type).  
- A **Caravan / Trailer specifications** section including:
  - Trailer type, tare, ATM, GTM (with “GTM ≈ ATM − ball weight”), ball weight, payload (ATM − tare)
  - Brakes type and axle count
  - Vehicle load inputs (passengers/cargo/roof load) in the V2 page

> Note: The tool is intended as a guide/selector — **always validate your numbers against manufacturer specs, compliance plates, and state rules**.

### 😠 The Grumpy Old Man Course
File:
- `GrumpyV1.html`

What it does:
- A humour page for “learning the ancient Aussie art of having a good whinge”.
- Offline “grump tools” like a rant starter and a polite→grumpy converter.
- Local progress tracking (stored on your device/browser).
- An optional “Cheeky AI Sidekick” section with configurable API settings (stored locally in the browser).

## Quick start (local)
1. Download/clone the repo
2. Open any of the `.html` files in your browser, e.g.
   - `Car SelectorV2.html`
   - `GrumpyV1.html`

That’s it.

## Hosting (GitHub Pages)
These are static pages — you can host them anywhere that serves static files:
- GitHub Pages
- Netlify / Cloudflare Pages
- Any basic web host

If using GitHub Pages:
1. Repo → **Settings** → **Pages**
2. Source: `Deploy from a branch`
3. Branch: `main` / root
4. Save, then use the Pages URL GitHub provides.

## Privacy notes
- These pages are designed to work **without logins**.
- Any progress/settings mentioned are stored **in your browser** (local storage / cache style behaviour).
- If you point the “Cheeky AI” feature at an API endpoint, requests will go to *that* endpoint (so treat API keys carefully — don’t embed secrets in public pages).

## Disclaimer (especially for towing)
This project is **not** legal advice, engineering certification, or a substitute for:
- tow-vehicle manufacturer limits
- caravan/trailer compliance plates
- state/territory regulations
- professional advice where required

Use it as a planning tool, then verify everything properly.

## Roadmap ideas (optional)
If you want to evolve this repo, good next steps could be:
- Add a proper landing `index.html` that links to each tool
- Add sample datasets / sources (and document where vehicle data comes from)
- Add “How to interpret towing numbers (ATM/GTM/GVM/GCM)” explainer
- Add unit tests (even lightweight JS checks) for calculation logic
- Add a licence

## Contributing
PRs and issues welcome:
- bug fixes
- UI improvements
- better copy / clearer disclaimers
- data source improvements and citations

## Licence
No licence file yet — default is “all rights reserved” until you add one.
Consider MIT if you want it broadly reusable.
