# Groff's Awards — Project Tracker
**groffsawards.com** | Launch Date: June 30, 2026

---

## Status: 🔴 Pre-Launch — DNS Broken

---

## The Mission
Emily Mankin retires from the family business June 30, 2026.
groffsawards.com needs to be ready to catch her.
This isn't just a website. It's her livelihood. Her second act.

---

## Team
| Role | Person |
|---|---|
| Owner / Operator | Emily Mankin |
| Architect / Strategist | The Professor (Claude Web) |
| Builder / Technical Partner | Stan 🦞 |
| Mission Control | Miguel |
| Coder (as needed) | Ed (Claude Code on linux-lab) |

---

## Technical Stack
| Component | Choice | Status |
|---|---|---|
| E-commerce | Shopify | Account exists, unused |
| DNS | Cloudflare → Shopify | ❌ 525 SSL error (BLOCKER) |
| Automation | n8n on conductor-01 | Ready |
| Photography | iPhone → Google Drive → Shopify | Workflow TBD |
| Scanning | ScanSnap iX2500 | On-site |

---

## Blockers
| # | Blocker | Owner | Status |
|---|---|---|---|
| 1 | Shopify admin access / credentials | Miguel | ⏳ Pending |
| 2 | Cloudflare API token or login for groffsawards.com | Miguel | ⏳ Pending |
| 3 | Emily's top 10-15 products (names + prices) | Emily | ⏳ Awaiting intro |
| 4 | Logo files (vector preferred) | Emily | ⏳ Awaiting intro |
| 5 | Brand colors | Emily | ⏳ Awaiting intro |

---

## Phase 1 — Foundation (Target: Week of March 22)
- [ ] Fix Cloudflare DNS → Shopify (525 SSL error)
  - Add groffsawards.com as custom domain in Shopify admin
  - Shopify generates SSL cert
  - Update Cloudflare DNS: CNAME @ → shops.myshopify.com
  - Set Cloudflare SSL mode to "Full"
- [ ] Activate Shopify store
- [ ] Choose and install theme (warm, artisan feel — TBD with Emily)
- [ ] Configure basic store settings (currency, shipping zones, taxes)
- [ ] Set up product collections structure:
  - Trophies & Trophy Cups
  - Plaques (wood, marble, glass)
  - Medals & Ribbons
  - Corporate Awards
  - Engraved Gifts
  - Custom Laser Engraving (as a service)

## Phase 2 — Product Catalog (Target: April)
- [ ] Receive Emily's top 10-15 products
- [ ] Build iPhone → Google Drive → auto-resize → Shopify photo workflow
- [ ] Load first 5-6 hero products with photos + descriptions
- [ ] Set up engraving customization options at checkout (text input, font choice, file upload)
- [ ] Pricing + variants for each product

## Phase 3 — Engraving Proof Workflow (Target: May — KEY DIFFERENTIATOR)
- [ ] Customer uploads artwork OR enters engraving text at checkout
- [ ] n8n picks up new order with engraving request
- [ ] Proof image generated and emailed to customer
- [ ] Customer clicks approve link → triggers production queue
- [ ] Emily gets production notification with all details
- [ ] Build approval UI (simple web page, mobile-friendly)

## Phase 4 — Full Automation via n8n (Target: June)
- [ ] New order → Emily notified (email + Telegram)
- [ ] Proof approval → production trigger
- [ ] Order shipped → tracking email to customer
- [ ] 30 days post-delivery → review request
- [ ] 11 months post-order → reorder reminder (corporate awards repeat annually — HIGH VALUE)

## Phase 5 — Launch Readiness (June 30)
- [ ] All hero products live with photos
- [ ] Proof/approval workflow tested end-to-end
- [ ] Payment processing confirmed (Shopify Payments or Stripe)
- [ ] Shipping rates configured
- [ ] Contact page + About Emily page
- [ ] Privacy policy + Terms (Shopify templates)
- [ ] Emily trained and comfortable
- [ ] LAUNCH 🚀

---

## Decisions Log
| Date | Decision | Made By |
|---|---|---|
| 2026-03-22 | Shopify as e-commerce platform | Pre-existing |
| 2026-03-22 | Cloudflare for DNS | Pre-existing |
| 2026-03-22 | n8n on conductor-01 for automation | Pre-existing |
| 2026-03-22 | Proof approval workflow = key differentiator | Professor |
| 2026-03-22 | Phase 1 sprint approved | Professor |
| 2026-03-22 | iPhone → Google Drive → Shopify photo workflow | Professor |
| 2026-03-22 | Emily gets direct Telegram line to Stan | Professor / Miguel |

---

## Completed
| Date | Item |
|---|---|
| 2026-03-22 | Project brief reviewed (conductor-system/projects/groffsawards/) |
| 2026-03-22 | groffsawards.com diagnosed — 525 SSL error, Shopify not connected |
| 2026-03-22 | teawithemily.com reviewed — already live, warm design, leave it alone |
| 2026-03-22 | Emily introduction message drafted and approved |
| 2026-03-22 | This PROJECT.md created |

---

## Notes
- **Reorder reminders are gold** — corporate awards repeat annually. 11-month reminder = easy revenue.
- **teawithemily.com** is live and beautiful. Don't touch it unless Emily asks. May add blog/tea reviews section later at her direction.
- ScanSnap iX2500 on-site — can also be used for digitizing any existing product documentation, order forms, etc.
- Emily currently takes product photos on iPhone — good enough for now, workflow makes it painless.
