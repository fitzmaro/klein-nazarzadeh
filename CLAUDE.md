# Klein & Nazarzadeh, PLLC — Website Project

## What This Is
Single-page landing page for a Manhattan personal injury law firm. Two attorneys (Klein & Nazarzadeh) leaving big law to start their own practice. No existing online presence.

## Live Info
- **Repo**: https://github.com/fitzmaro/klein-nazarzadeh
- **Firm Address**: 1675 Broadway, 14th Floor, New York, NY 10019
- **Firm Name**: Klein & Nazarzadeh, PLLC
- **Hosting**: Not yet set up (plan: GitHub Pages)
- **Domain**: KNinjurylaw.com (purchased on GoDaddy, username: 129118019)

## Tech Stack
- Single `index.html` file (all CSS/JS inline)
- Google Fonts: DM Serif Display (headings), Plus Jakarta Sans (body)
- No framework, no build step — just open the file
- JSON-LD structured data for local SEO

## Design Decisions
- **Aesthetic**: Architectural luxury — warm cream (#F5F0EB) and near-black (#0A0A0A) with muted brass gold (#B8956A)
- **Typography**: DM Serif Display for display text (swapped from Bodoni Moda which was too thin on screen), Plus Jakarta Sans for body
- **Film grain overlay** via SVG feTurbulence filter
- **Giant decorative `&`** watermark in hero background
- **Practice areas** are an interactive accordion list (not cards)
- **Scroll animations**: clip-path line-mask reveals on hero headline, IntersectionObserver fade-ups elsewhere
- **Scrolling marquee** strip between hero and about section
- Reference sites used for copy inspiration (not design): jknylaw.com, perecman.com, shulman-hill.com, unionlawfirm.com

## Page Sections (in order)
1. **Nav** — fixed, transparent → solid on scroll, hamburger on mobile
2. **Hero** — full viewport, massive headline "Your Injury. Our Fight.", stats bar at bottom, scroll hint
3. **Marquee** — horizontal scrolling strip with key messages
4. **About** — their story of leaving big law, pull quote, two attorney cards
5. **Practice Areas** — accordion list (motor vehicle, construction, premises liability, medical malpractice, wrongful death, workplace injuries)
6. **Why Us** — bordered grid: no fee, direct access, big law training, proven results
7. **No Fee Strip** — gold accent banner
8. **Contact** — left: address/phone/email, right: consultation form
9. **Footer** — minimal with legal disclaimers

## TODOs (marked with `TODO` comments in the HTML)
- [ ] Replace phone number placeholder `(212) 000-0000` with real number (appears in nav, mobile menu, contact section, footer)
- [ ] Replace email `info@kleinnazarzadeh.com` with real email (contact section, footer)
- [ ] Update attorney cards with first names and real bios
- [ ] Wire up form submission to a backend (Formspree, Netlify Forms, or custom)
- [ ] Set up GitHub Pages hosting and point GoDaddy DNS (A records → GitHub IPs, CNAME www → fitzmaro.github.io, add CNAME file to repo)
- [ ] Set up firm email — clients need to buy Microsoft 365 Business Basic ($6/user/mo) through GoDaddy, then create mailboxes (klein@, nazarzadeh@, info@). Note sent to clients explaining options.
- [ ] Update structured data URL from `kleinnazarzadeh.com` to actual domain
- [ ] Add real phone number to JSON-LD structured data
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
- Once they purchase M365 through GoDaddy, create: klein@, nazarzadeh@, info@kninjurylaw.com
