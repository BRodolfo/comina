# Image Manifest

Downloaded from Figma file `KCEZQrhodUoRVEE14cUJJq` into `public/assets/images/`. All 16 downloads succeeded (no failures, no placeholders needed).

| Filename | Type (verified) | Pixels | Size | Figma node | Used in | Status |
|---|---|---|---|---|---|---|
| hero-background.jpg | JPEG | 2560×1707 (resized) | 183 KB | 1:18 | Hero background (shown 1646×1097, offset −136/−151, cover) | OK |
| about-image.jpg | JPEG | 1600×1067 (resized) | 254 KB | 1:51 | About photo (779×528, radius 16) | OK |
| testimonials-image.jpg | JPEG | 1024×683 (converted from PNG) | 89 KB | 1:90 | Testimonials photo (610×528, radius 16, object-bottom) | OK |
| logo-comira.svg | SVG | 28×28 | 1.6 KB | 1:691 | Navbar logo | OK |
| footer-logo-comira.svg | SVG | 68.4×68.4 | 1.7 KB | 1:163 | Footer logo | OK |
| icon-personal-bag.svg | SVG | 48×48 | 1.2 KB | 1:68 | Benefits: Personalized Training | OK |
| icon-barbell.svg | SVG | 48×48 | 1.8 KB | 1:73 | Benefits: On-Demand Workouts | OK |
| icon-egg.svg | SVG | 48×48 | 1.9 KB | 1:78 | Benefits: Nutrition Guidance | OK |
| icon-fitness.svg | SVG | 48×48 | 2.2 KB | 1:83 | Benefits: Progress Tracking | OK |
| icon-quote.svg | SVG | 48×48 | 0.3 KB | 1:93 | Testimonials quote mark | OK |
| icon-arrow-prev.svg | SVG | 12×24 | 0.5 KB | 1:99 | Testimonials "previous" button (Figma flips it) | OK |
| icon-arrow-next.svg | SVG | 12×24 | 0.5 KB | 1:103 | Testimonials "next" button | OK |
| icon-arrow-faq.svg | SVG | 12×24 | 0.5 KB | 1:116 | FAQ toggle buttons (Figma rotates it 90°) | OK |
| icon-twitter-x.svg | SVG | 24×24 | 0.5 KB | 1:189 | Footer social | OK |
| icon-instagram.svg | SVG | 24×24 | 1.5 KB | 1:193 | Footer social | OK |
| icon-facebook.svg | SVG | 24×24 | 0.4 KB | 1:199 | Footer social | OK |

## Notes
- Figma exported `hero-background` and `about-image` as JPEG data with a `.png` name. Both were renamed to `.jpg`.
- Phase 5 optimization: the originals were 4096×2731 (hero 2.1 MB, about 9.5 MB) and the testimonial photo was a 1.1 MB PNG. They were resized/recompressed to the sizes above (about 13 MB down to about 0.5 MB total). Re-export from Figma if full-resolution originals are needed.
- Testimonial photo: Figma stretches the whole frame to the 610×528 slot (no crop), so the CSS uses `object-fit: fill` to match the design.
- Hero Image Placeholder (`1:568`) is an empty 100×100 frame and was not exported.
