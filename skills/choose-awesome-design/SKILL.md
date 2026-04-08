---
name: choose-awesome-design
description: Use when user wants to design UI, build a prototype, or establish visual style for a project. Guides user through design style selection via multi-turn conversation, scanning project docs first, then recommending brand-inspired design systems from VoltAgent/awesome-design-md.
---

# Awesome DESIGN.md — Design Style Advisor

Help users pick the right design system through structured discovery, then fetch the DESIGN.md from GitHub.

## Step 1: Scan Project Documents

Before asking the user anything, scan the current project for context. Look for:

- `README.md`, `AGENTS.md`, `CLAUDE.md` — project overview and purpose
- Files with names containing: `prd`, `requirement`, `spec`, `design`, `architecture`, `overview`, `brief` (any extension, especially `.md`)
- `package.json` — to infer tech stack and product type
- Any other `.md` files in the project root or `/docs` folder

Read whatever you find. Extract:
- **What the product does** (type, purpose, core features)
- **Who the target users are** (developers, consumers, enterprise, creatives, etc.)
- **Any mentioned visual preferences or brand references**
- **Technical stack** (web app, mobile, dashboard, marketing site, etc.)

If no documents found, note that and proceed to Step 2.

## Step 2: Multi-Turn Discovery Conversation

Ask questions across these 4 dimensions. **Do not dump all questions at once** — ask 1-2 at a time, listen, follow up naturally. Reference what you found in Step 1.

### Dimension 1: Target Users
- Who will use this product? (developers, business users, consumers, creatives, general public)
- What's their context? (professional tool, casual app, high-stakes financial, creative expression)

### Dimension 2: Product Type & Industry
- What category? (SaaS dashboard, AI tool, fintech, e-commerce, docs/content platform, marketing site, mobile app)
- Any specific industry constraints? (finance needs trust signals, healthcare needs clarity, automotive needs premium feel)

### Dimension 3: Visual Atmosphere
- Light or dark? Or system-adaptive?
- Dense/information-rich or spacious/minimal?
- Tone: professional/serious, friendly/approachable, bold/edgy, elegant/premium, technical/precise
- Color preferences or things to avoid?

### Dimension 4: Reference & Constraints
- Any brands, apps, or sites the user finds inspiring? (even outside the catalog)
- Any existing brand colors or assets to respect?
- Anything they explicitly want to avoid?

## Step 3: Recommend 2-3 Design Systems

After gathering enough context (usually 3-5 exchanges), synthesize everything and recommend **2-3 options** from the catalog below.

For each recommendation, provide:
- **Why it fits** — connect back to what the user said and what you found in their docs
- **Best for** — specific scenarios where this shines
- **Watch out for** — where it might fall short for their use case

Then ask: *"Which feels closest? Or should I explore other directions?"*

## Step 4: Fetch and Apply

Once user confirms a choice, fetch the DESIGN.md using:

```
https://raw.githubusercontent.com/VoltAgent/awesome-design-md/main/design-md/{folder}/DESIGN.md
```

Read the full content and use it as the authoritative design spec for all UI work in this session.

---

## Brand Catalog

### Design & Productivity
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| Airtable | `airtable` | Colorful, friendly, structured data aesthetic |
| Cal.com | `cal` | Clean neutral, developer-oriented simplicity |
| Clay | `clay` | Organic shapes, soft gradients, art-directed |
| Figma | `figma` | Vibrant multi-color, playful yet professional |
| Framer | `framer` | Bold black/blue, motion-first, design-forward |
| Intercom | `intercom` | Friendly blue, conversational UI patterns |
| Miro | `miro` | Bright yellow accent, infinite canvas feel |
| Notion | `notion` | Warm minimalism, serif headings, soft surfaces |
| Pinterest | `pinterest` | Red accent, masonry grid, image-first |
| Webflow | `webflow` | Blue-accented, polished marketing site |

### Developer Tools
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| Cursor | `cursor` | Dark IDE aesthetic, precision tooling |
| Expo | `expo` | React Native ecosystem, clean documentation |
| HashiCorp | `hashicorp` | Enterprise infra, structured navy palette |
| Linear | `linear.app` | Speed-focused, ultra-minimal dark UI |
| Mintlify | `mintlify` | Documentation-first, clean white |
| MongoDB | `mongodb` | Green-accented, developer-friendly |
| Ollama | `ollama` | Minimal terminal-inspired |
| PostHog | `posthog` | Bold dark analytics, hedgehog brand |
| Raycast | `raycast` | macOS launcher aesthetic, dark premium |
| Replicate | `replicate` | ML platform, clean technical |
| Resend | `resend` | Email API, minimal developer-focused |
| Sanity | `sanity` | Red accent, structured content management |
| Sentry | `sentry` | Error tracking, purple dark mode |
| Supabase | `supabase` | Green-black, open-source Postgres energy |
| Vercel | `vercel` | Black/white precision, deployment-focused |
| Warp | `warp` | Modern terminal, dark gradient |

### AI & ML
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| Claude | `claude` | Warm amber, thoughtful conversational |
| Cohere | `cohere` | Coral accent, AI-forward |
| ElevenLabs | `elevenlabs` | Dark audio-focused, waveform aesthetic |
| Lovable | `lovable` | Friendly purple, generative UI |
| MiniMax | `minimax` | Clean AI platform |
| Mistral | `mistral.ai` | French AI, clean minimal |
| OpenCode | `opencode.ai` | Developer AI tooling |
| Runway | `runwayml` | Creative AI, cinematic dark |
| Together AI | `together.ai` | Open AI infrastructure |
| VoltAgent | `voltagent` | AI agent framework |
| X.AI | `x.ai` | Grok/xAI, minimalist black |

### Fintech & Crypto
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| Coinbase | `coinbase` | Clean blue, institutional trust-focused |
| Kraken | `kraken` | Purple dark UI, data-dense dashboards |
| Revolut | `revolut` | Sleek dark, gradient cards, fintech precision |
| Stripe | `stripe` | Purple gradient, polished developer fintech |
| Wise | `wise` | Bright green accent, friendly and clear |

### Enterprise & Consumer
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| Airbnb | `airbnb` | Warm coral, photography-driven, rounded UI |
| Apple | `apple` | Premium white space, SF Pro, cinematic |
| IBM | `ibm` | Carbon design system, structured blue |
| NVIDIA | `nvidia` | Green-black energy, technical power |
| SpaceX | `spacex` | Stark black/white, full-bleed imagery |
| Spotify | `spotify` | Vibrant green on dark, bold type |
| Superhuman | `superhuman` | Speed-focused email, dark premium |
| Uber | `uber` | Bold black/white, tight type, urban energy |
| Zapier | `zapier` | Orange accent, workflow automation |

### Automotive
| Brand | Folder | Style Signature |
|-------|--------|-----------------|
| BMW | `bmw` | Dark premium surfaces, German precision |
| Ferrari | `ferrari` | Chiaroscuro black-white editorial, Ferrari Red |
| Lamborghini | `lamborghini` | True black cathedral, gold accent |
| Renault | `renault` | Aurora gradients, NouvelR typeface |
| Tesla | `tesla` | Radical subtraction, cinematic viewport |

---

## Quick Matching Heuristics

Use these when making recommendations:

| User Context | Strong Candidates |
|---|---|
| Developer tool / API product | Vercel, Linear, Supabase, Resend, Warp |
| AI / LLM product | Claude, Cohere, ElevenLabs, Mistral, Runway |
| SaaS dashboard (B2B) | Linear, Notion, PostHog, Sentry, IBM |
| Consumer app (B2C) | Airbnb, Spotify, Pinterest, Intercom |
| Fintech / crypto | Stripe, Revolut, Coinbase, Kraken, Wise |
| Marketing / landing page | Apple, Framer, Webflow, Vercel, Tesla |
| Content / docs platform | Notion, Mintlify, Sanity, Cal.com |
| Creative / design tool | Figma, Miro, Clay, Framer |
| Premium / luxury feel | Apple, Ferrari, Lamborghini, Tesla, Superhuman |
| Friendly / approachable | Airtable, Intercom, Notion, Wise, Zapier |
