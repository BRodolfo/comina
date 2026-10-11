# Site Map

**Figma File Key**: `KCEZQrhodUoRVEE14cUJJq`
**Source URL**: `https://www.figma.com/design/KCEZQrhodUoRVEE14cUJJq/comira?node-id=1-16&m=dev`
**Container Max-Width**: `1440px` (frame 1440; content 1320px with 60px side padding)

The Figma file has one page and one frame (`Design`, 1440 × 4971). It is a **single-page landing site**, so there is one route: `/`.

## Pages

### Page: Home
Node ID: `1:16`

#### Sections

| Section | Node ID | Component | Background | Notes |
|---------|---------|-----------|------------|-------|
| Navbar | `1:711` (def. `1:699`) | Navbar | transparent, overlays hero | Absolute at y=20, 1320 wide. Logo + "Comira" left, pill button "Temlis" right. Collapse to menu ≤991px only if needed |
| Hero | `1:17` | Hero | `#02071a` + full-bleed photo | 923 tall. Photo `1646×1097` at (−136, −151), cover. Contents vertically centered: heading left, glass signup card (424 wide) right |
| About | `1:47` | About | black | 988 tall, 100px padding. 72px heading, photo 779×528 left, text + 2 stats right |
| Benefits | `1:61` | Benefits | black | 636 tall. Centered headline + 4-column features, 100px gap |
| Testimonials | `1:88` | Testimonials | black | 728 tall. Photo 610×528 left, quote + prev/next buttons right (vertically centered), 100px gap |
| FAQ | `1:106` | Faq | black | 1180 tall. Centered header + 872px-wide list of 5 items, 40px gap |
| Footer | `1:152` | Footer | black | 516 tall, **52px** side padding, 80px vertical. Newsletter + logo row, then links / contact / social row |

#### Section internals (for Phase 2)
- **Hero** `1:19` Main Content → `1:20` Heading (Anton 120/1.2, "Get early" white, "access" `#cfff13`); `1:21` Signup Container → `1:22` Countdown Timer, `1:30` Description, `1:31` Email Signup (with `1:661` Button)
- **About** `1:48` Content Container → `1:49` Heading, `1:50` Image and Text Container → `1:51` Image, `1:52` Text Container (`1:53` Description, `1:54` Stats: `1:55`, `1:58`)
- **Benefits** `1:62` → `1:63` Headline Container (`1:64`, `1:65`), `1:66` Features Container → `1:67`, `1:72`, `1:77`, `1:82`
- **Testimonials** `1:89` → `1:90` Image, `1:91` Quote Container → `1:92` (quote `1:95`, author `1:96`), `1:97` Navigation Buttons (`1:98` prev, `1:102` next)
- **FAQ** `1:107` → `1:108` Header (`1:109`, `1:110`), `1:111` List → `1:112`, `1:120`, `1:128`, `1:136`, `1:144`
- **Footer** `1:153` Newsletter (`1:154`, logo `1:162`); `1:167` Links (`1:168`) / Contact (`1:179`: details `1:180`, social `1:185`)

## Layout Analysis
| Section | Background spans | Content max-width | Decorative |
|---|---|---|---|
| Hero | Full viewport (photo cover, oversized) | 1320 | None |
| About | Full viewport (black) | 1320 | None |
| Benefits | Full viewport | 1320 | None |
| Testimonials | Full viewport | 1320 | None |
| FAQ | Full viewport | 872 list / 1320 container | 1px white bottom border per item |
| Footer | Full viewport | 1336 (52px padding) | None |

## Shared Components
| Component | Node ID | Description |
|-----------|---------|-------------|
| Button (pill) | `1:661`, `1:695`, `1:158` | `#cfff13` fill, 48px pill, Inter 600 12px uppercase, 1.44px tracking. 40px high in navbar, 48px in forms |
| Round icon button | `1:98`, `1:102`, `1:115`, `1:188` | 40px (slider, FAQ) / 48px (social), `#cfff13` fill |
| Email field (glass pill) | `1:31`, `1:156` | 64px high, 64px radius, 8% white fill, 1px 8% white border, 20px blur, button inside right |
| Glass card | `1:21`, `1:22` | 8% white fill, 1px 8% white border, 20px blur, radius 16 / 12 |
| Highlight heading | `1:49`, `1:64`, `1:109` | Anton 72/80, uppercase, white with `#cfff13` accent words |
| Feature item | `1:67` … | 48px icon, Anton 24/32 title, Inter 16/24 body in `#c3c3c3`, centered |
| FAQ item | `1:112` … | Question row (Anton 24/32) + toggle button, answer below (Inter 16/24, `#c3c3c3`) |
| Logo | `1:691`, `1:163` | Comira mark + Anton wordmark (navbar 28px, footer 68.4px) |

## Components to build (Astro)
`Navbar.astro`, `Hero.astro`, `About.astro`, `Benefits.astro`, `Testimonials.astro`, `Faq.astro`, `Footer.astro`, plus atoms `Button.astro`, `EmailField.astro`, `IconButton.astro`.

## Design tokens observed
See `PROJECT_BRIEF.md` and `src/styles/global.css`.
