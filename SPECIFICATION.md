# Tempisque Tech Website Specification

## Overview

A minimal, one-page static website for Tempisque Tech, a professional services company with operations in the UK and USA. The site will be clean, concise, and bank-friendly while meeting regulatory requirements for both jurisdictions.

---

## Company Information

### Entities

| Entity | Jurisdiction | Registration |
|--------|--------------|--------------|
| TEMPISQUE TECH LIMITED | United Kingdom | Company Number: 15942273 |
| TEMPISQUE TECHNOLOGY COMPANY | United States (Delaware) | Delaware LLC |

### Addresses

**UK Office:**
128 City Road
London, EC1V 2NX
United Kingdom

**US Office:**
Tempisque Technology Company
2261 Market Street STE 85081
San Francisco, CA 94114
United States

### Contact

- **Email:** contact@tempisque.tech
- **Website:** https://tempisque.tech

---

## Founder

**Boaz Sobrado, Founder**

### External Profiles
- Personal website: https://boazsobrado.com/
- Forbes: https://www.forbes.com/sites/boazsobrado/
- LinkedIn: https://www.linkedin.com/in/boazsobrado/
- Podcast (On The Margin): https://www.on-the-margin.com/

---

## Services

**Professional Services**

The services description should remain deliberately concise and generic to avoid bank payment processing issues. The site should describe the company as offering:

> "Professional Services"

This encompasses the actual business activities:
- Advisory/consulting for fintech and crypto companies
- Media services (podcast clipping campaigns)
- Content creation (Forbes contributor)

**Note:** Do NOT list specific service categories on the website. Keep the description bank-friendly and generic.

---

## Design Specification

### Style Guide

**Inspiration:** Edward Tufte's design principles
- Reference: https://edwardtufte.github.io/tufte-css/

**Key Design Principles:**
- Minimal and clean aesthetic
- High readability with excellent typography
- White/light background
- Generous whitespace
- No unnecessary decorative elements
- Content-first approach

### Typography

Following Tufte CSS conventions:
- Serif font for body text (e.g., et-book, Palatino, Georgia)
- Clean hierarchy with subtle distinctions
- Comfortable line height and measure

### Logo

Generate a simple, minimal text-based logo for initial launch. Requirements:
- Clean, professional appearance
- Works in monochrome
- Scalable (vector preferred)
- Placeholder for future branded logo

### Color Palette

Minimal palette inspired by Tufte:
- Background: Off-white (#fffff8 or similar)
- Text: Dark gray/black (#111 or similar)
- Accent: Subtle, muted (if needed)
- Links: Distinguished but not garish

---

## Page Structure

### Single Page Layout

```
┌─────────────────────────────────────┐
│           HEADER / LOGO             │
├─────────────────────────────────────┤
│                                     │
│           COMPANY NAME              │
│           & TAGLINE                 │
│                                     │
├─────────────────────────────────────┤
│                                     │
│           ABOUT / SERVICES          │
│     (Professional Services)         │
│                                     │
├─────────────────────────────────────┤
│                                     │
│           FOUNDER                   │
│     Boaz Sobrado, Founder           │
│     [Social/Profile Links]          │
│                                     │
├─────────────────────────────────────┤
│                                     │
│           CONTACT                   │
│     contact@tempisque.tech          │
│                                     │
├─────────────────────────────────────┤
│                                     │
│           LOCATIONS                 │
│     UK Address | US Address         │
│                                     │
├─────────────────────────────────────┤
│           FOOTER                    │
│  Company registrations, legal links │
└─────────────────────────────────────┘
```

---

## Legal & Compliance Pages

### Required Pages

1. **Privacy Policy** (`/privacy` or `/privacy.html`)
2. **Terms of Service** (`/terms` or `/terms.html`)

### Privacy Policy Requirements

Must address:
- GDPR compliance (UK/EU users)
- Data collection disclosure (Mixpanel analytics)
- Cookie usage (if any)
- User rights
- Contact information for data requests

### Terms of Service Requirements

Must include:
- Service description
- Limitation of liability
- Governing law (specify UK and/or US jurisdiction)
- Intellectual property
- Contact information

### Footer Compliance Information

Display in footer:
- UK: "TEMPISQUE TECH LIMITED is registered in England and Wales. Company No. 15942273"
- US: "TEMPISQUE TECHNOLOGY COMPANY is a Delaware LLC"
- Links to Privacy Policy and Terms of Service
- Copyright notice

---

## Analytics & Tracking

### Services to Integrate

1. **Mixpanel** - User analytics
2. **Google Search Console** - SEO monitoring (meta tag verification)

### Cookie Consent

Since Mixpanel collects user data, a cookie consent banner may be required for GDPR compliance. Consider:
- Simple, non-intrusive banner
- Clear accept/decline options
- Link to privacy policy

---

## Technical Specification

### Technology Stack

- **Type:** Static HTML/CSS website
- **Hosting:** GitHub Pages
- **Domain:** tempisque.tech
- **SSL:** Enabled via GitHub Pages

### File Structure

```
/
├── index.html          # Main single-page site
├── privacy.html        # Privacy Policy
├── terms.html          # Terms of Service
├── css/
│   └── style.css       # Tufte-inspired styles
├── images/
│   └── logo.svg        # Company logo
└── README.md           # Repository documentation
```

### Performance Requirements

- Fast loading (< 2 seconds)
- No JavaScript frameworks required
- Minimal dependencies
- Mobile responsive

### SEO Requirements

- Proper meta tags (title, description)
- Open Graph tags for social sharing
- Structured data (Organization schema)
- robots.txt
- sitemap.xml

---

## Responsive Design

### Breakpoints

- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

### Mobile Considerations

- Stacked layout for addresses
- Readable typography at all sizes
- Touch-friendly link targets

---

## Content Checklist

### Must Have
- [ ] Company name and logo
- [ ] "Professional Services" description
- [ ] Founder name and title
- [ ] UK address with company number
- [ ] US address with entity info
- [ ] Contact email
- [ ] External profile links (4 links)
- [ ] Privacy Policy page
- [ ] Terms of Service page
- [ ] Footer with legal registrations
- [ ] Copyright notice

### Nice to Have
- [ ] Subtle animations on load
- [ ] Print stylesheet
- [ ] Dark mode toggle

---

## Deployment

### GitHub Pages Setup

1. Repository: `tempisque_tech_static_site` (or similar)
2. Branch: `main` or `gh-pages`
3. Custom domain: tempisque.tech
4. HTTPS: Enforced

### DNS Configuration

Configure at domain registrar:
- A records pointing to GitHub Pages IPs
- CNAME for www subdomain (if needed)

---

## Summary

| Attribute | Value |
|-----------|-------|
| Type | Single-page static site + 2 legal pages |
| Design | Tufte-inspired minimal |
| Hosting | GitHub Pages |
| Domain | tempisque.tech |
| Contact | contact@tempisque.tech |
| Analytics | Mixpanel, Google Search Console |
| Legal | Privacy Policy, Terms of Service |
| Compliance | GDPR, UK Companies Act, US disclosure |
