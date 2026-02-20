# GLP-1 Weight Loss Clinic — Landing Page Template

A premium, single-file landing page template for medical weight loss clinics.

## Quick Start

1. Open `index.html` in a browser
2. Edit the `CONFIG` object at the top of the `<script>` section:

```javascript
const CONFIG = {
  businessName: 'Your Clinic Name',
  tagline: 'Your Tagline',
  phone: '(555) 123-4567',
  email: 'hello@yourclinic.com',
  address: '123 Main St, City, ST 12345',
  startPrice: '$179',
  refillPrice: '$299',
  ctaUrl: '#intake',
};
```

## Customization Guide

### Colors
All colors are CSS variables at `:root`. Change them directly or use the built-in **Theme Switcher** (bottom-left button) to preview 10 pre-built palettes.

To set a permanent default theme, update the `:root` variables in the `<style>` block.

### Content
Search for `<!-- CHANGE:` comments throughout the HTML to find every editable element:
- Headline, subheadlines, checklist items
- Product names, prices, and tags
- Testimonials and review quotes
- FAQ questions and answers
- Doctor names and credentials
- Contact information

### Images
Replace placeholder boxes with real images:
1. Search for elements with classes like `photo-grid-item`, `result-photo`, `doctor-avatar`, `product-img`
2. Replace the emoji/background with `<img>` tags or CSS `background-image`
3. Keep the existing border-radius and overflow styles

### Data Arrays (in JavaScript)
- `FAQ_DATA` — Questions and answers
- `RESULTS_DATA` — Before/after patient results
- `REVIEWS_DATA` — Customer reviews
- `THEMES` — Color theme definitions

### Adding Your Logo
Replace the text logo in the navbar:
```html
<a href="#" class="nav-logo">Your Logo Here</a>
<!-- Or use an image: -->
<a href="#"><img src="logo.png" alt="Logo" style="height:32px;"></a>
```

### Form Integration
The intake form (`#intakeForm`) currently shows an alert on submit. To connect it:
- Replace the `submit` event handler with your form endpoint (Typeform, Jotform, custom API, etc.)
- Or replace the entire `<form>` with an embedded form iframe

## Technical Details
- **Single file** — all CSS and JS embedded, no build step
- **~57KB** — fast loading
- **Mobile-first responsive**
- **No dependencies** except Google Fonts (Red Hat Text)
- **10 color themes** built in with live switching
- **Smooth animations** — scroll fade-in, counter animations, carousel auto-scroll

## Sections (in order)
1. Sticky Navigation
2. Hero + Photo Grid
3. Logo Slider (As Seen In)
4. Product Cards
5. Results Carousel
6. Featured Testimonial
7. Interactive Weight Calculator
8. The Change (Stats + Grid)
9. Why Patients Sign Up (Stats)
10. 3-Step Journey
11. Support/Care Section
12. Extended Reviews
13. FAQ Accordion
14. Money-Back Guarantee
15. Doctor Profiles
16. Footer
17. Sticky Mobile CTA
18. Intake Form Modal
