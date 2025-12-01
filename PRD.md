# Miki Electrical Services Landing Page PRD

## 1. Overview
- **Product**: One-page marketing site promoting Miki Electrical Services in South Ethiopia.
- **Purpose**: Showcase expertise, services, and contact options while providing a polished, mobile-friendly presence.
- **Deployment Targets**: GitHub Pages (public repo) and Vercel (for optimized CDN delivery).

## 2. Objectives & Success Metrics
| Objective | KPI | Target |
| --- | --- | --- |
| Ensure business credibility | Page live on GitHub Pages & Vercel | Both URLs published |
| Increase lead generation | CTA click-through rate | ≥ 10% of visits |
| Provide performance baseline | Core Web Vitals (LCP, CLS) | LCP < 2.5s, CLS < 0.1 |

## 3. Stakeholders
- **Business Owner**: Miki / Minas Behayilu – final approvals.
- **Designer/Developer**: Cascade assistant + user – implementation and polish.
- **Ops**: User (GitHub + Vercel account owner) – handles DNS, repo, deployments.

## 4. Target Users
| Persona | Needs |
| --- | --- |
| Homeowners (South Ethiopia) | Trustworthy electrician, quick contact, service list |
| Business owners / property managers | Commercial reliability, project showcase |
| Partners / suppliers | Proof of professionalism, brand identity |

## 5. Requirements
### 5.1 Functional
1. **Hero** with headline, subheadline, hero image, CTA buttons (Call Now, Request Service) and phone number.
2. **About** section describing credentials and hero imagery.
3. **Services** listing four categories with icons & hover states.
4. **Showcase** grid featuring 10 project images with zoom/hover animation.
5. **Why Choose Us** bullet grid with icons.
6. **Contact** section including phone (+251926038769), location (Dilla, South Ethiopia), email (minasbehayilu@gmail.com), availability and buttons (Call / Send Message).
7. Smooth scrolling & section navigation from sticky header.
8. Scroll-triggered animations on key content blocks.

### 5.2 Non-Functional
- **Branding**: Manrope font, deep blue headings, white background, yellow accents.
- **Responsiveness**: Optimized for mobile-first with flexible grids.
- **Performance**: Static HTML/CSS/JS, optimized images (PNG/JPG from provided assets).
- **Accessibility**: Semantic HTML, descriptive alt text, sufficient color contrast.
- **Reliability**: Hosted redundantly on GitHub Pages and Vercel.

## 6. Design References
- Hero background: `images/hero-electrician.png` overlayed with gradient.
- Imagery: `images/electrician2.png`, `images/logo.png`, `images/showcase1-10.jpg`.
- Animation approach: CSS transitions + IntersectionObserver.

## 7. Deployment Plan
### GitHub Pages
1. Create repo (e.g., `miki-electrical-site`) and push `index.html` + `images/` + `PRD.md`.
2. In repo Settings → Pages, set Source = `main` branch, `/ (root)` directory.
3. Verify at `https://<username>.github.io/miki-electrical-site/`.
4. Optional: add custom domain DNS + `CNAME` file when ready.

### Vercel
1. Import the same GitHub repo in Vercel dashboard.
2. Framework preset: “Other” (static). Build command: `npm run build` (leave empty) or `null`; Output dir: `.`.
3. Deploy and confirm Vercel URL (e.g., `https://miki-electrical.vercel.app`).
4. Configure custom domain (optional) and ensure HTTPS edge caching.

### Tracking
- Maintain checklist via GitHub Issues or Projects for: repo setup, Pages publish, Vercel deploy, DNS/custom-domain tasks.
- Capture deployment URLs in README or PRD under a “Links” section once live.

## 8. Risks & Mitigations
| Risk | Mitigation |
| --- | --- |
| Large image assets reduce performance | Compress images or use WebP in future iteration |
| DNS misconfiguration for custom domain | Document DNS records, verify via `dig` before switching |
| Asset path issues between hosts | Keep relative paths consistent, avoid host-specific configs |

## 9. Timeline (suggested)
| Task | Owner | Due |
| --- | --- | --- |
| Repo + asset push | User | Day 0 |
| GitHub Pages enablement | User | Day 0 |
| Vercel import + deploy | User | Day 0 |
| Post-launch QA (cross-browser/mobile) | User | Day 1 |
|

## 10. Open Questions
1. Will a custom domain be attached immediately?
2. Any analytics requirement (e.g., Google Analytics) to add?
3. Need for contact form backend or integrations in future iteration?
