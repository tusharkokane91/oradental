# Ora Dental Clinic — SEO Optimization Plan

**Website:** oradental.in  
**Business Type:** Local Service (Dental Clinic)  
**Location:** Baner, Pune, Maharashtra 411045  
**Doctor:** Dr. Shivani Gujarathi Dagadu  
**Created:** 2026-03-02  

---

## Current SEO Audit Summary

| Category | Status | Notes |
|----------|--------|-------|
| Meta Tags | ⚠️ Basic | Title & description exist, missing OG/Twitter |
| Structured Data | ❌ None | No JSON-LD, no schema at all |
| robots.txt | ❌ Missing | No crawl directives |
| sitemap.xml | ❌ Missing | No XML sitemap |
| Canonical URL | ❌ Missing | No self-referencing canonical |
| Open Graph | ❌ Missing | No social sharing metadata |
| Accessibility | ⚠️ Partial | Some ARIA labels, needs improvement |
| Performance | ✅ Good | Static site, minimal JS, lazy-loaded map |
| Mobile | ✅ Good | Responsive, viewport meta present |
| HTTPS | ✅ Good | GitHub Pages enforces HTTPS |
| Image Alt Text | ⚠️ Basic | Alt tags exist but not keyword-optimized |
| Semantic HTML | ✅ Good | Proper section/nav/footer usage |
| E-E-A-T Signals | ⚠️ Weak | Doctor name present but no credentials/schema |
| Local SEO | ⚠️ Weak | Address present but no LocalBusiness schema |
| AI/GEO Readiness | ❌ None | No llms.txt, no AI crawler config |

**Current Score: ~30/100** — Lots of low-hanging fruit!

---

## Phase 1 — Foundation (Quick Wins) 🔥

*Estimated effort: 2-3 hours. Immediate impact.*

### 1.1 Structured Data (JSON-LD)
Add the following schema markup to `index.html`:

- **Dentist (LocalBusiness subtype)** — name, address, phone, hours, geo coordinates, priceRange, image
- **Person** — Dr. Shivani with credentials (BDS, etc.)
- **WebSite** — site name, URL, search action
- **BreadcrumbList** — even for single-page, helps search engines
- **Service** — for each dental service offered

### 1.2 Meta Tags Overhaul
- **Canonical URL:** `<link rel="canonical" href="https://oradental.in/">`
- **Open Graph tags:** og:title, og:description, og:image, og:url, og:type, og:locale
- **Twitter Card tags:** twitter:card, twitter:title, twitter:description, twitter:image
- **Enhanced description:** More keyword-rich, include "dentist in Baner Pune"
- **Geo meta tags:** geo.region, geo.placename, geo.position
- **Language:** Confirm `lang="en"` + add `hreflang` self-reference

### 1.3 robots.txt
Create `/robots.txt` with:
- Allow all search engines
- Reference sitemap.xml
- Allow AI crawlers (GPTBot, PerplexityBot, ClaudeBot) for AI search visibility
- Block training-only crawlers (Bytespider, CCBot)

### 1.4 sitemap.xml
Create `/sitemap.xml` with the single page URL + lastmod date.

### 1.5 llms.txt (AI Search Visibility)
Create `/llms.txt` for AI crawlers with structured clinic info.

---

## Phase 2 — Content & E-E-A-T Enhancement 📝

*Estimated effort: 3-4 hours. Medium-term ranking boost.*

### 2.1 Doctor Credentials (E-E-A-T Critical)
- Add **BDS degree** and registration number to the About section
- Add **years of experience** with specifics
- Add **professional affiliations** (IDA - Indian Dental Association, etc.)
- This is **YMYL (Your Money or Your Life)** content — health! Google requires strong E-E-A-T.

### 2.2 Enhanced Service Descriptions
Each service card currently has ~15-20 words. For SEO:
- Create **dedicated anchor sections** per service (e.g., `#root-canal`, `#teeth-whitening`)
- Expand descriptions to **100-150 words** with keywords like:
  - "best root canal treatment in Baner Pune"
  - "teeth whitening cost in Pune"
  - "dental implants near me Baner"
  - "pediatric dentist Baner Pune"

### 2.3 FAQ Section
Add a FAQ section with common patient questions:
- "What are the clinic hours?"
- "Do you accept dental insurance?"
- "How much does a root canal cost in Pune?"
- "Is teeth whitening safe?"
- "What age should children first visit a dentist?"

*Note: FAQ schema is restricted to healthcare authority sites only (as of Aug 2023), so we add the content but NOT the FAQPage schema.*

### 2.4 Testimonials/Reviews Section
- Add a reviews section with patient testimonials
- Include **AggregateRating** schema for the clinic
- Link to Google Reviews for social proof

### 2.5 Image Optimization
- Add keyword-rich alt text: "Dr. Shivani Gujarathi dental clinic Baner Pune"
- Compress images (logo.jpg is 30KB ✅, dr-shivani.jpg is 490KB ⚠️ — compress!)
- Add `width` and `height` attributes to prevent CLS
- Consider WebP format for better performance

---

## Phase 3 — Technical SEO 🔧

*Estimated effort: 2-3 hours. Improves crawlability and Core Web Vitals.*

### 3.1 Performance Optimization
- **Preload critical assets:** hero image, fonts
- **Defer non-critical CSS:** Font Awesome can be loaded async
- **Image compression:** dr-shivani.jpg needs to go from 490KB → <100KB
- **Add `width`/`height`** to all `<img>` tags (prevents CLS)
- **Font display swap:** Already using `display=swap` ✅

### 3.2 Security Headers
If custom hosting (not just GitHub Pages):
- Content-Security-Policy
- X-Content-Type-Options: nosniff
- Referrer-Policy: strict-origin-when-cross-origin

### 3.3 Accessibility Improvements (WCAG 2.2 AA)
- Ensure all interactive elements have **focus indicators**
- Check **color contrast** ratios (brown on light bg should be fine)
- Add **skip-to-content** link
- Ensure **touch targets** are ≥48x48px
- Add `role` attributes where needed

### 3.4 IndexNow
- Submit to Bing/Yandex via IndexNow for faster non-Google indexing

---

## Phase 4 — Local SEO & Off-Page 🗺️

*Ongoing effort. Critical for local dental searches.*

### 4.1 Google Business Profile
- Ensure **NAP consistency** (Name, Address, Phone) matches website exactly
- Add all **service categories** (Dentist, Cosmetic Dentist, Pediatric Dentist)
- Upload **clinic photos** regularly
- Respond to all **reviews** (positive and negative)
- Post **weekly updates** (tips, offers, before/after)
- Video verification if not done
- Keep **business hours accurate** (top-5 ranking factor!)

### 4.2 Local Directory Listings
- **Justdial** — Claim/update listing
- **Practo** — Doctor profile with services and fees
- **Sulekha** — Business listing
- **Google Maps** — Already present ✅
- **Apple Maps** — Submit listing
- **Bing Places** — Claim listing

### 4.3 Review Strategy
- Ask happy patients to leave Google Reviews
- Target **50+ reviews** with **4.5+ average rating**
- Respond to every review within 24 hours

### 4.4 Social Media Presence
- Create **Instagram** account (dental before/after photos)
- Create **Facebook** page
- Add social links to website + schema `sameAs`

---

## Target Keywords

### Primary Keywords (High Intent)
| Keyword | Search Intent | Priority |
|---------|--------------|----------|
| dentist in Baner Pune | Local discovery | 🔴 High |
| dental clinic Baner | Local discovery | 🔴 High |
| best dentist Baner Pune | Local + quality | 🔴 High |
| Ora Dental Clinic | Brand | 🔴 High |

### Secondary Keywords (Service-Specific)
| Keyword | Priority |
|---------|----------|
| root canal treatment Baner Pune | 🟡 Medium |
| teeth whitening Pune | 🟡 Medium |
| dental implants Baner | 🟡 Medium |
| braces cost Pune | 🟡 Medium |
| pediatric dentist Baner | 🟡 Medium |
| emergency dentist Pune | 🟡 Medium |

### Long-Tail Keywords
| Keyword | Priority |
|---------|----------|
| painless root canal near Baner | 🟢 Low |
| best cosmetic dentist Pune | 🟢 Low |
| dental clinic near Zudio Baner | 🟢 Low |
| affordable dental treatment Pune | 🟢 Low |

---

## Implementation Checklist

### Phase 1 — Do Now ✅
- [ ] Add JSON-LD structured data (Dentist, Person, WebSite)
- [ ] Add canonical URL
- [ ] Add Open Graph meta tags
- [ ] Add Twitter Card meta tags
- [ ] Add geo meta tags
- [ ] Create robots.txt
- [ ] Create sitemap.xml
- [ ] Create llms.txt
- [ ] Optimize meta description with local keywords
- [ ] Compress dr-shivani.jpg
- [ ] Add width/height to all images

### Phase 2 — This Week 📝
- [ ] Add doctor credentials to About section
- [ ] Enhance service descriptions with keywords
- [ ] Add FAQ section
- [ ] Add testimonials section
- [ ] Optimize all image alt text
- [ ] Add skip-to-content link

### Phase 3 — This Month 🔧
- [ ] Preload critical assets
- [ ] Defer non-critical CSS
- [ ] Submit to IndexNow
- [ ] Full accessibility audit
- [ ] Core Web Vitals testing

### Phase 4 — Ongoing 🗺️
- [ ] Optimize Google Business Profile
- [ ] Submit to local directories
- [ ] Build review volume
- [ ] Create social media profiles
- [ ] Monthly content updates

---

## KPI Targets

| Metric | Now | 3 Months | 6 Months |
|--------|-----|----------|----------|
| Google "dentist Baner Pune" | Not ranked | Top 20 | Top 10 |
| Google Business Profile views | Unknown | 500/mo | 1500/mo |
| Organic Traffic | ~0 | 100/mo | 500/mo |
| Google Reviews | Unknown | 30+ | 50+ |
| Core Web Vitals | Unknown | All green | All green |
| Schema Validation | ❌ Fail | ✅ Pass | ✅ Pass |

---

## Notes

- This is a **YMYL site** (health/dental) — E-E-A-T is critical
- **Dental clinic SEO in India** is competitive but local searches in Baner are achievable
- The site is static (GitHub Pages) which is great for performance
- Consider expanding to multi-page in the future (blog, individual service pages)
- AI Search (GEO) optimization is low priority for local dental but good to future-proof
