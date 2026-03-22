# PROJECTS.md — Active Projects

Last updated: 2026-03-22

---

## 🏆 Priority 1: groffsawards.com
**Status:** DNS broken (525 error) — Shopify not connected to Cloudflare  
**Deadline:** June 30, 2026 (Emily's retirement from family business)  
**Owner:** Emily (co-owner with Professor)  
**Stan's role:** Builder and business partner

### What Emily Does
Laser engraving, trophies, plaques, medals, ribbons, custom awards on wood/glass/metal/acrylic. Physical store, existing inventory.

### Technical Stack
- Shopify (account exists, unused)
- Cloudflare DNS → Shopify (pending — THIS IS THE BLOCKER)
- n8n on conductor-01 (automation ready)
- ScanSnap iX2500 (on-site, for product photo workflow)

### Phase 1 Sprint (approved by Professor)
- [ ] Fix Cloudflare DNS → Shopify (525 error = SSL misconfiguration)
- [ ] Activate Shopify store, choose theme
- [ ] Load 5-6 hero products
- [ ] Basic n8n: new order → Emily notified
- [ ] Proof workflow skeleton

### Photography Workflow (to build)
iPhone photo → Google Drive folder → auto-resize/optimize → Shopify upload

### Key Differentiator
Proof approval before production. Customer uploads text/art → proof emailed → customer approves → production queue triggers.

### Automation Pipeline (n8n)
1. New order → Emily notified
2. Proof approval → production trigger
3. Shipped → tracking email
4. 30 days post-delivery → review request
5. 11 months post-order → reorder reminder (high value — corporate awards repeat annually)

### Assets Needed
- [ ] Logo (vector preferred)
- [ ] Brand colors
- [ ] Top 10-15 products from Emily
- [ ] Product photography

---

## 🍵 Priority 2: teawithemily.com
**Status:** LIVE — beautiful site already built on Cloudflare  
**Owner:** Emily  
**What it is:** Warm conversation/interview show — Emily sits with elders, longtime locals, people with stories worth preserving. Tea, two mugs, a lifetime of memories.  
**Format:** YouTube @teawithemilyshow, Instagram @teawithemilyshow  
**Contact:** emily@teawithemily.com

### What's needed (TBD — ask Emily)
- Does she want a blog/writing component added?
- Episode archive / show notes pages?
- She mentioned "tea reviews and life after teaching" — that might be a new section

### Stan's approach
Her voice, her pace. Don't over-engineer. Enhance what's already beautiful.

---

## 💧 WaterBase (waterbase.app)
**Status:** Planning  
**Stack:** FastAPI + PostgreSQL + React + Tailwind  
**Brief:** ~/projects/waterbase/CLAUDE.md

---

## ⚽ FollowMySports (followmysports.com)
**Status:** Planning  
**Team:** Grant (sports marketing), Evan (golf), Miguel (product)  
**Stack:** FastAPI + PostgreSQL + React + SportsRadar API  
**Brief:** ~/projects/followmysports/CLAUDE.md

---

## 📋 Other
- hmg-coatesville-va — ~/projects/hmg-coatesville-va/
- nest-hub-dashboard — ~/projects/nest-hub-dashboard/
- Groff family business sale — MikeMankin/groff-sale (context only, not a build project)
