# Skill: Landing Page Builder

## Purpose
Creates high-converting landing pages for event registrations, product inquiries, lead magnets, and campaign-specific offers. Outputs as a self-contained HTML file.

## When to Use
- Event registration pages (Modern Medicine Symposium, Art of the Eyes)
- Product interest capture pages
- Lead magnet download pages
- Campaign-specific landing pages

## Inputs Required
- **Page goal**: Registration, lead capture, information, or download
- **Target audience**: Practice type(s) and their key motivations
- **Event/product details**: What's being promoted
- **Form fields needed**: Name, email, practice, phone, specialty, etc.
- **Brand version**: Modern Medicine Symposium or Art of the Eyes

## Page Structure
```
1. HERO SECTION
   - Headline: Clear value proposition (what they get)
   - Subheadline: Supporting detail (when, where, why it matters)
   - Primary CTA button
   - Hero image or event visual

2. BENEFITS SECTION
   - 3-4 key reasons to attend/engage
   - Icons or visual elements for each
   - Practice-type specific benefits

3. AGENDA / DETAILS
   - Event schedule or product details
   - Speaker highlights or treatment information
   - What they'll walk away with

4. SOCIAL PROOF
   - Past event testimonials
   - Practice success stories
   - Attendance numbers or device installation count

5. REGISTRATION / CONTACT FORM
   - Minimal fields (reduce friction)
   - Clear submit CTA
   - Privacy note

6. FOOTER
   - BTL Aesthetics branding
   - Contact: Aalia Mohammad
   - Event logistics (address, parking, dates)
```

## Design Guidelines
- Clean, modern, professional design
- BTL brand colors and fonts
- Mobile-responsive layout
- Fast loading (minimal external dependencies)
- Accessible (proper contrast, alt text, semantic HTML)

## Technical Output
- Single self-contained HTML file with inline CSS
- No external dependencies except CDN fonts if needed
- Form can submit to a placeholder action (to be connected to HubSpot)
- Include Open Graph meta tags for social sharing

## Quality Checks
- [ ] Headline clearly communicates value
- [ ] CTA is visible above the fold
- [ ] Form fields are minimal and appropriate
- [ ] Mobile responsive
- [ ] Correct event branding (Symposium vs Art of the Eyes)
- [ ] No em dashes in copy
- [ ] Contact information is accurate
