# Klein & Nazarzadeh, PLLC — Website Project

## What This Is
Single-page landing page for a Manhattan personal injury law firm. Two founding partners (Kevin Klein and Jordan Jacob Nazarzadeh) plus two Of Counsel attorneys (Alan Chester Salzman, Harvey Alan Winer).

## Live Info
- **Live URL**: https://kninjurylaw.netlify.app
- **Repo**: https://github.com/fitzmaro/klein-nazarzadeh
- **Netlify admin**: https://app.netlify.com/projects/kninjurylaw
- **Firm Address**: 1675 Broadway, 14th Floor, New York, NY 10019
- **Phone**: (212) 540-3311
- **Email**: info@kninjurylaw.com
- **Domain**: KNinjurylaw.com (purchased on GoDaddy — see credentials in password manager, not here)
- **Hosting**: Netlify (deployed, live)

## Tech Stack
- Single `index.html` file (all CSS/JS inline)
- Google Fonts: DM Serif Display (headings), Plus Jakarta Sans (body)
- No framework, no build step — just open the file
- JSON-LD structured data for local SEO
- Deployed via `netlify deploy --dir=. --prod`

## Design Decisions
- **Aesthetic**: Architectural luxury — warm cream (#F5F0EB) and near-black (#0A0A0A) with muted brass gold (#B8956A)
- **Typography**: DM Serif Display for display text (swapped from Bodoni Moda which was too thin on screen), Plus Jakarta Sans for body
- **Film grain overlay** via SVG feTurbulence filter
- **Giant decorative `&`** watermark in hero background
- **Practice areas** displayed as a 4-column bordered grid (20 items)
- **Scroll animations**: clip-path line-mask reveals on hero headline, IntersectionObserver fade-ups elsewhere
- **Scrolling marquee** strip between hero and about section
- **Contact**: mailto CTA button (no form) — opens email client with pre-filled template
- Reference sites used for copy inspiration (not design): jknylaw.com, perecman.com, shulman-hill.com, unionlawfirm.com

## Attorneys
- **Kevin Klein, Esq.** — Founding Partner. Hofstra Law. Admitted in NY, SDNY, EDNY. Super Lawyers 2018–2025 (badge embedded).
- **Jordan Jacob Nazarzadeh, Esq.** — Founding Partner. NY Law School. Admitted in NY, NJ.
- **Alan Chester Salzman, Esq.** — Of Counsel
- **Harvey Alan Winer, Esq.** — Of Counsel

## Practice Areas (20)
Car Accidents, Motorcycle Accidents, Truck Accidents, Bus Accidents, Pedestrian Accidents, Bicycle Accidents, Construction Accidents, Workplace Accidents, Premises Liability, Slip & Fall, Medical Malpractice, Product Liability, Labor Law, Negligent Security, Brain Injuries, Child Injuries, Assault Injuries, Dog Bite Injuries, Defective Drugs & Medical Devices, Immigration Law

## Page Sections (in order)
1. **Nav** — fixed, transparent → solid on scroll, hamburger on mobile
2. **Hero** — full viewport, massive headline "Your Injury. Our Fight.", stats bar at bottom, scroll hint
3. **Marquee** — horizontal scrolling strip with key messages
4. **About** — their story of leaving big law, pull quote, full attorney profiles with bios/education/admissions, Of Counsel cards
5. **Practice Areas** — 4-column grid of 20 practice areas
6. **Why Us** — bordered grid: no fee, direct access, big law training, proven results
7. **No Fee Strip** — gold accent banner
8. **Contact** — left: address/phone/email, right: mailto CTA button + phone link
9. **Footer** — three required legal disclaimers (Attorney Advertising, Results Disclaimer, No Attorney-Client Relationship)

## TODOs
- [ ] Connect GoDaddy domain to Netlify (add custom domain in Netlify dashboard, point GoDaddy nameservers to Netlify)
- [ ] Set up firm email — clients need to buy Microsoft 365 Business Basic ($6/user/mo) through GoDaddy, then create mailboxes. Note sent to clients in `email-note-to-client.md`, awaiting their decision.
- [ ] Add favicon

## Client Requirements (from their brief)
- Over $50 million recovered for clients
- Licensed to practice in New York State
- Decades of combined experience
- Color scheme: black, white, silver (we went with black, warm cream, brass gold — more premium)
- No verdicts taken — they said not to highlight this
- Goals: clean website, hosting, firm email setup with Outlook

## Email Situation
- Clients want @kninjurylaw.com emails in Outlook
- No free option exists for custom domain email (Gmail or Outlook)
- Recommended: Microsoft 365 Business Basic via GoDaddy ($6/user/mo, DNS auto-configured)
- Alternative: Google Workspace ($7/user/mo) but they prefer Outlook
- Note sent to clients in `email-note-to-client.md` explaining options, awaiting their decision
- Once they purchase M365 through GoDaddy, create: kevin.klein@, jordan.nazarzadeh@, info@kninjurylaw.com
