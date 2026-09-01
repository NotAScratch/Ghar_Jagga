# Ghar Jagga – Product Thinking Notes (Nepal Real Estate)

This repository now captures a practical planning baseline for a Nepal-focused real estate web app inspired by Zillow, PropertyShark, MagicBricks, and 99acres.

## 1) Non-negotiable feature set (and Nepal priority)

### Must-have at launch
- **Search + map browsing** with filters: city/area, buy/rent, property type, price (NPR), bedroom, land area (ropani/aana + sq ft/m²), furnished/unfurnished.
- **Listing detail pages** with strong media: photos first, then facts, map, nearby landmarks.
- **Account basics**: save listings, shortlists, recent searches.
- **Alerts**: instant + daily digest for saved searches (high-retention pattern used by Zillow/99acres).
- **Lead capture**: call, WhatsApp/Viber link, and in-app inquiry.
- **Seller/agent listing submission flow** with guided forms and moderation queue.
- **Bilingual UI foundation**: English + Nepali (Unicode), language toggle persistent per user.
- **Nepal payment rails** for monetization flows: **eSewa** and **Khalti**.

### High-value soon after launch
- **Verified badges** (owner/agent/doc-checked) to build trust.
- **Agent profile pages** (active listings, response rate, locality focus).
- **Price insights lite** (median asking price by area and type; not full AVM early).
- **Project pages** for developers (new apartment/housing projects).

### Later / optional
- 3D tours, advanced valuation engine, deep legal workflow automation, investor analytics dashboards.

## 2) User flows and friction to remove

### Buyers / Renters
1. Landing → filter search → map/list compare  
2. Open listing → trust checks (verification, freshness, agent info)  
3. Save / contact / schedule visit

**Friction to solve:** stale listings, missing price, poor photos, slow agent response.  
**Borrowed pattern:** Zillow-style saved search alerts + 99acres-style locality-centric discovery.

### Sellers / Owners
1. Create account → choose owner/agent listing  
2. Guided form (smart defaults, unit conversions) → upload photos  
3. Optional paid boost via eSewa/Khalti → publish after moderation

**Friction to solve:** complex forms, uncertainty on fair price, low lead quality.

### Agents / Brokers
1. Profile setup + KYC/verification  
2. Bulk listing management  
3. Lead inbox + response tracking + paid visibility

**Friction to solve:** proving credibility and managing follow-up speed.

### Investors
1. Explore hotspots by city/ward  
2. Compare yields/asking trends (basic first)  
3. Contact local experts

## 3) Trust + monetization model

### Trust mechanisms (critical in Nepal context)
- **Listing freshness policy** (auto-expire unless reconfirmed every X days).
- **Mandatory structured fields** (price, location precision tier, ownership type).
- **Verification states**: phone verified, identity verified, document reviewed.
- **Report listing** + moderation SLA.
- **Agent reputation signals**: response time, deal activity, user ratings (post-transaction where possible).

### Monetization (startup-feasible)
- **Freemium listings** (limited free posts/month).
- **Premium boosts** (top-of-search, locality spotlight, homepage slots).
- **Agent subscription tiers** (lead credits, CRM-lite, branding).
- **Project marketing packages** for developers.
- Optional later: mortgage/referral partnerships.

## 4) Nepal-specific adaptation (what global templates miss)

- **Location granularity**: Province → District → Municipality/Metro → Ward.
- **Local land units** first-class (ropani, aana, daam, bigha/kattha/dhur by region).
- **Price communication norms**: total NPR + “per aana/per sq ft” toggles.
- **Connectivity context**: road access type, water source, electricity reliability.
- **Document context fields**: lalpurja/document readiness metadata (without over-promising legal validity).
- **Language behavior**: mixed Nepali/English search terms (Romanized Nepali support later).
- **Urban/rural listing quality variance**: stronger moderation and assisted onboarding outside major cities.

## 5) MVP scope: credible minimum vs later

### MVP (build now)
- Auth + profiles
- Search + filters + map/list
- Listing creation + moderation
- Saved listings + saved search alerts
- Inquiry/contact flow
- Basic verification badges
- Bilingual UI + NPR + local area units
- eSewa/Khalti payment for featured listing
- Admin panel (approve/reject listings, flag handling)

### Phase 2
- Agent subscription plans
- Locality price trend charts
- User reviews/ratings
- Developer project pages

### Phase 3
- Advanced valuation models
- Financing eligibility tools
- Virtual tours at scale

## Prioritization tradeoff guidance

- If forced to choose, prioritize **trust + freshness + contact conversion** over flashy intelligence features.
- A weak valuation model hurts less than fake/stale listings.
- Payments should be integrated early only for simple boosts/subscriptions, not full transactional closing.
- Keep data models extensible (units, verification states, role types), but keep first release UX short and guided.