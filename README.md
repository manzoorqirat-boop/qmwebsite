# QMSofts Website

Static marketing site for **QMSofts** — a software studio building AI-built,
cloud-hosted management platforms for specific industries. Served as a static
site at **qmsofts.com** (see `CNAME`), suitable for GitHub Pages or any static host.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — hero, product grid, foundation/values, CTA |
| `products.html` | Full product catalogue, one detailed block per product |
| `about.html` | Studio story, principles, industries served |
| `contact.html` | Demo-request form with industry picker |
| `styles.css` | Shared theme (CSS variables: `--ink`, `--gold`, `--emerald`, …) |
| `favicon.svg` | Brand Q-mark favicon |
| `robots.txt`, `sitemap.xml` | Search-engine crawl + index hints |
| `CNAME` | Custom domain (`qmsofts.com`) |

No build step, no framework — plain HTML/CSS with Google Fonts. Each page is
self-contained; navbar and footer are duplicated per page (edit all pages when
changing either).

## Products featured

Seven platforms, each AI-built, multi-tenant and cloud-hosted:

1. **QMSoft School OS** — schools (admissions, attendance, exams, fees, payroll; bilingual EN/हिंदी)
2. **Dawa** — pharmacies (batch/expiry stock, OCR capture, purchase→sales, analytics)
3. **Restel** — hotels (PMS, bookings, housekeeping, POS, OTA sync)
4. **Nidan** — pathology labs (patients, test catalogue, samples, reports, billing)
5. **QMH** — hospitals & nursing homes *(added — see below)*
6. **QMO** — distributors (order portal, AI order-parsing, dispatch, margins)
7. **QMfg** — small factories (BOM→production→finished goods, full finance/P&L/GST)

## What QMH is (the new product)

A hospital management system covering the full patient journey, OPD to discharge:

- **OPD** — appointment → vitals → prescriptions → billing as one staged live queue
- **IPD** — ward & bed allocation, automatic daily bed charges, discharge summaries
- **Billing** — server-side invoices; prescription→bill and discharge→bill (bed
  charges auto-settled for the whole stay); consumables billable to a patient
- **Clinical masters** — configurable vital standards, diagnoses, medicines with
  composition, dosages, durations, routes, tests, instructions
- **Inventory** — general consumables with stock in/out, low-stock alerts
- **Analytics & reports** — NABH-style MIS (occupancy/ALOS/revenue), birthday and
  monthly reports
- **Platform** — role-based access, multi-tenant row-level isolation, audit trails

On the site QMH is the fifth product block (between Nidan and QMO), with a matching
home-page card and entries in every nav/footer list.

## Changes in this revision

**Added QMH across the site**
- Product block on `products.html` (badge **H**, Hospital · Healthcare)
- Product card on `index.html` grid
- Industry value tile on `about.html`
- Footer "Products" lists updated on all pages
- "Hospital — QMH" option in the contact-form industry picker
- Copy updated "six" → "seven" platforms/industries; "hospitals" added to industry
  lists in hero, blurbs and meta descriptions; new "Hospital" chip in the kicker strip

**Site-wide improvements**
- **Favicon** (`favicon.svg`) using the brand Q-mark — previously none
- **SEO/social meta** on every page: canonical URL, Open Graph + Twitter Card tags,
  and `theme-color`
- **`robots.txt`** + **`sitemap.xml`** for crawling/indexing

## Next steps

- Add `og-cover.png` (1200×630) referenced by the social-preview tags; until then
  the tags are present but the image 404s gracefully.
- Navbar/footer are copy-pasted per page; if you add an 8th product, update all four
  pages plus this README.