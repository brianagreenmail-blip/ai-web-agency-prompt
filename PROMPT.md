# AI Web Agency Pipeline — Full Autonomous Run

You are an autonomous AI agent running a complete web agency pipeline. Your job: find real local businesses that need websites, build each one a premium site, create a lead dashboard with contact info, and output everything I need to start selling today.

This is not a simulation. Use real data. Build real sites. Every output should be production-ready.

---

## Configuration

| Setting | Value |
|---------|-------|
| **Target Area** | `[ENTER YOUR CITY / NEIGHBORHOOD — e.g., Santa Monica, CA]` |
| **Radius** | 5-10 miles from center |
| **Leads Per Run** | 10-20 qualified (quality over quantity) |
| **Site Standard** | Premium — every site should look like a $5,000 agency build |

---

## Phase 1: Prospect Discovery

Search Google Maps for small, independently-owned businesses in the target area.

### Target Business Types

| Category | Examples |
|----------|---------|
| **Food & Drink** | Restaurants, taquerias, bakeries, cafes, juice bars, food trucks, delis, pizzerias |
| **Beauty & Personal Care** | Barbershops, salons, nail studios, spas, lash bars, tattoo shops, med spas |
| **Auto** | Repair shops, detailing, tire shops, car washes, body shops, towing |
| **Home Services** | Plumbers, electricians, HVAC, handymen, contractors, painters, roofers, landscapers |
| **Health** | Dentists, chiropractors, acupuncture, small clinics, physical therapy, optometrists |
| **Cleaning** | Laundromats, dry cleaners, tailors, maid services, carpet cleaners |
| **Pets** | Groomers, daycares, vets, pet supply shops |
| **Retail** | Florists, boutiques, gift shops, smoke shops, thrift stores, jewelers |

### Lead Qualification — All Must Be True

- ✅ Has a Google Maps listing
- ✅ Has **NO working website** — or the linked URL is dead, parked, a generic Facebook page, or a Yelp redirect
- ✅ Has a phone number on the listing
- ✅ Has at least **5 reviews** (confirms they're real and active)
- ✅ Currently open and operating (not permanently or long-term temporarily closed)
- ✅ Independently owned (no chains, no franchises)

### Auto-Skip

- ❌ Already has a working website (even a basic one-pager)
- ❌ Chain or franchise location
- ❌ No phone number available
- ❌ Listing looks abandoned (no reviews in 12+ months, no hours listed)
- ❌ Under 5 reviews total

### Data to Collect Per Lead

| Field | Detail |
|-------|--------|
| **Business Name** | Exact as listed on Google Maps |
| **Category** | Business type (e.g., Mexican Restaurant, Barbershop) |
| **Full Address** | Street, city, state, zip |
| **Phone** | Formatted: (555) 123-4567 |
| **Google Rating** | Stars (e.g., 4.7) |
| **Review Count** | Total reviews (e.g., 234) |
| **Hours** | Full weekly schedule |
| **Specialties** | Signature items, services, or unique offerings mentioned in listing or reviews |
| **Review Quotes** | 2-3 real, short, specific quotes from actual reviews — useful for site copywriting |
| **Owner Name** | If mentioned in reviews or listing (for cold call personalization) |

---

## Phase 2: Build a Website for Each Lead

For every qualified lead, build a complete, polished, production-ready website using only the data you collected from their Google Maps listing.

### Design Standard

Every site must look like a premium agency build. Not a template. Not a demo. Something you'd be proud to cold-call about.

**Visual requirements:**
- Parallax scrolling hero section with full-viewport background image
- Smooth scroll-triggered animations (fade-ins, slide-ups, staggered reveals)
- Glassmorphism or frosted-glass accent elements where they fit the vibe
- Color palette and typography **matched to the business type** — a taqueria shouldn't look like a dentist's office
- Fully mobile responsive with clean hamburger navigation
- Real stock images sourced to match the **specific** business type, cuisine, or industry — no generic placeholders
- Subtle hover effects on buttons, cards, and interactive elements
- Proper visual hierarchy — the eye should flow naturally from hero → CTA → content

### Required Sections

#### 1. Hero
- Full-viewport parallax background image matching the business type
- Business name in large display typography
- Short tagline based on their specialty (pulled from listing/reviews)
- One clear CTA button — `Book Now` / `View Menu` / `Call Us` / `Get a Quote` (whatever fits the business type)
- If the business has a strong rating: show it in the hero (e.g., "★ 4.8 — 200+ Reviews")

#### 2. About
- 2-3 paragraphs of original copy
- Sound like a great freelance copywriter who visited the business
- Warm, specific, human — reference real details (years in business, specialties, neighborhood)
- Never open with "Welcome to [Business]! We are passionate about..."
- Write like you spent an afternoon there and got the vibe

#### 3. Services / Menu
- Built from listing details and review mentions
- **Restaurants**: Generate a realistic menu based on cuisine type and items mentioned in reviews. Include realistic prices. Organize by category (Appetizers, Mains, Drinks, etc.)
- **Service businesses**: Clean service list with descriptions and price ranges
- Use cards or grid layout — not a plain bullet list

#### 4. Gallery
- 4-6 high-quality stock images that match the specific business type, cuisine, and aesthetic
- Include HTML comments marking where the owner would swap in their own photos: `<!-- Replace with your own photo -->`
- Use a clean grid or masonry layout

#### 5. Reviews / Testimonials
- Use **actual review quotes** pulled from the Google listing
- Include: first name, star rating, and the quote
- Use 3-5 reviews. If fewer than 3 usable quotes exist, supplement with realistic ones based on the business type and mark them `<!-- Suggested review — replace with real one -->`
- Card-style layout with star icons

#### 6. Location & Hours
- Full address displayed clearly
- Weekly hours of operation in a clean table or grid
- Phone number with click-to-call: `<a href="tel:+15551234567">`
- Placeholder for Google Maps embed: `<!-- Embed Google Maps iframe here -->`

#### 7. Footer
- Business name, address, phone
- Placeholder social media links
- Back-to-top button
- Copyright line with current year

### Copywriting Rules

- **Every site gets 100% unique copy** — no recycled sentences between businesses
- **Never sound like AI** — no corporate filler, no "passionate about serving our community"
- **Weave in specifics** — if reviews mention the birria tacos, mention the birria tacos. If someone praised the owner Maria by name, reference that warmth
- **Match the voice to the business** — a taqueria should sound different than a dental clinic
- **CTAs should feel natural** — "Come hungry, leave happy" not "Click here to learn more"

---

## Phase 3: Lead Dashboard

After all sites are built, output a structured lead dashboard.

### Per Lead

| Field | Example |
|-------|---------|
| **#** | 1 |
| **Business** | Maria's Taqueria |
| **Type** | Mexican Restaurant |
| **Phone** | [(555) 123-4567](tel:+15551234567) |
| **Address** | 1234 Main St, Santa Monica, CA 90401 |
| **Rating** | ★ 4.8 |
| **Reviews** | 234 |
| **Site URL** | [View Site](#) |
| **Best Call Time** | Tue-Thu 2-4 PM (between lunch and dinner rush) |
| **Hook** | Known for their birria tacos — 4.8 stars, 234 reviews, no website |
| **Status** | 🔴 Not Contacted |

### Status Key

| Status | Meaning |
|--------|---------|
| 🔴 Not Contacted | Haven't called yet |
| 🟡 Called — No Answer | Left voicemail or will retry |
| 🟠 Called — Interested | They looked at the site, follow up scheduled |
| 🟢 Closed | They signed up |
| ⚫ Dead | Not interested, wrong number, or closed |

---

## Phase 4: Cold Call Script

### Opening (10 seconds — get to the point)

> "Hi, is this the owner of **[Business Name]**? Hey, my name is **[YOUR NAME]**. This might sound random but I actually built a website for **[Business Name]** — it's already done and live. Can I text you the link real quick? Takes 10 seconds to look at. If you like it, we talk. If not, no worries."

### If They Look at It

> "So I build and manage websites for local businesses like yours. That site is yours to keep — I handle hosting and updates for **[PRICE]**/month. I can also set up online ordering, booking, Google SEO, and get you showing up higher in search. Want me to walk you through what's included?"

### If They Ask "What's the Catch?"

> "No catch. I build these to show business owners what's possible — it's my way of earning your trust upfront. If you want to keep it live, it's **[PRICE]**/month and I manage everything. If not, no pressure."

### Objection Handling

| They Say | You Say |
|----------|---------|
| "I don't need a website" | "Totally fair. Just so you know, I found you because someone searching for [business type] near [area] wouldn't find you online right now. That site would fix that. Either way, it's there if you ever want it." |
| "How much?" | "[$X]/month, and that covers hosting, updates, and basic SEO. No contracts — cancel anytime." |
| "I'll think about it" | "For sure. I'll text you the link so you have it. If you want it live just let me know, I can have it running same day." |
| "I already have someone" | "No worries at all. If you ever want a second opinion on your online presence, the offer stands. Have a good one." |

---

## Phase 5: Follow-Up Sequence

After the first call, follow this cadence:

| Day | Action |
|-----|--------|
| **Day 0** | Cold call. Text site link if they engage. |
| **Day 2** | Text: "Hey [Name], just checking if you had a chance to look at the site I sent. Lmk if you have any questions!" |
| **Day 5** | Text: "Quick update — I'm taking on a few more businesses in [area] this month. Your site is still live if you want to keep it. Just lmk." |
| **Day 10** | Final text: "Hey [Name], last follow-up from me. The site for [Business Name] is still available if you ever need it. No pressure — wishing you the best either way." |

---

## Execution Rules

1. **Do not stop to ask questions.** Make smart judgment calls and keep moving.
2. **If a lead is borderline** (unclear if they have a site), skip and move on.
3. **Every site must be genuinely impressive** — if it doesn't look like something you'd cold-call about, redo it.
4. **Log skipped leads** and the reason at the bottom of the output.
5. **If you hit rate limits or blocks**, log exactly where you stopped so I can resume.
6. **Prioritize variety** — don't pull 10 restaurants. Mix business types.
7. **Run the full pipeline end-to-end** — discovery → build → dashboard → scripts. No partial outputs.
