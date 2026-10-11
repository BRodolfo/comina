# Project Brief — Comira

**Source**: https://www.figma.com/design/KCEZQrhodUoRVEE14cUJJq/comira?node-id=1-16
**Figma File Key**: `KCEZQrhodUoRVEE14cUJJq`
**Framework**: Astro (TypeScript strict)
**Design frame**: `Design` (`1:16`), 1440 × 4971 — single-page landing site
**Content width**: 1320px (60px side padding; Footer uses 52px)

## Project name
Comira — corporate fitness / wellness platform (waitlist landing page, copy references "Peloton Corporate Wellness").

## Brand colors
| Role | Hex | Figma token |
|---|---|---|
| Accent / primary button / highlight text | `#cfff13` | Colors/Button/Primary, Colors/Text/Text Yellow |
| Hero background (behind photo) | `#02071a` | — |
| Section background | `#000000` | — |
| Text — title (white) | `#ffffff` | Colors/Text/Text tittle white |
| Text — body on dark | `#c3c3c3` | Colors/Text/Text body dark |
| Button label (on accent) | `#131313` | — |
| Glass surface fill | `rgba(255,255,255,0.08)` | Colors/Background/Bg Black 2 |
| Glass outline | `rgba(255,255,255,0.08)` | Colors/Outline/Soft Gray |
| FAQ divider | `#ffffff` (1px) | — |

## Typography
- **Header font**: Anton, Regular (400), always uppercase — Google Fonts
- **Body font**: Inter, Regular 400 / SemiBold 600 — Google Fonts

| Style | Font | Size | Line-height | Letter-spacing | Use |
|---|---|---|---|---|---|
| Display | Anton | 120px | 1.2 | 0 | Hero "Get early access" |
| Headings/Text-5xl | Anton | 72px | 80px (1.111) | 0 | Section headings, stat values |
| Countdown | Anton | 40px | normal | 0 | Timer digits |
| Headings/Text-xl | Anton | 24px | 32px (1.333) | 0 | Feature titles, quote, FAQ questions, newsletter title |
| Logo (navbar) | Anton | 18.667px | 28px (1.5) | 0 | "Comira" |
| Logo (footer) | Anton | 45.608px | 68.412px (1.5) | 0 | "Comira" |
| Body/Text-base | Inter 400 | 16px | 24px (1.5) | 0 | Body copy |
| Footer heading | Inter 400 | 20px | 28px (1.4) | 0 | Directly to / Our Office / Follow Us |
| Button label | Inter 600 | 12px | 16px (1.333) | 1.44px | Uppercase |

## Spacing system
Tokens: `spacing/0` 0, `spacing/1` 4, `spacing/2` 8, `spacing/6` 24.
Common values: 4, 8, 12, 14, 16, 24, 40, 48, 64, 80, 100 (section padding and gap).
- Sections: 100px vertical padding, 60px horizontal (Footer 80px / 52px)
- Heading→content gap inside sections: 100px
- Hero signup card: padding 24px, gap 40px

## Border radius
4 unused; values: **12px** (countdown), **16px** (images, signup card), **48px** (pill buttons), **64px** (email input pill).

## Shadows
None. The glass surfaces use `backdrop-filter: blur(20px)` with the 8% white fill and outline instead.

## Design frame width
1440px → `--size-container-ideal: 1440`, `--size-container-max: 1440px`.

## Sections (top → bottom)
Navbar (overlay) · Hero · About · Benefits · Testimonials · FAQ · Footer

## Special interactions (implied by structure — only what the design shows)
- **Countdown timer** (160 : 21 : 01 : 59) in the hero signup card
- **Email signup** forms: hero ("Join Waitlist") and footer ("Subscribe")
- **Testimonial slider**: prev / next arrow buttons (single quote shown)
- **FAQ accordion**: round arrow button per question (all five shown in the design with answers visible)
- Social icon links: X, Instagram, Facebook
- No hover, scroll or parallax effects are specified — none will be added.

## Component patterns
- **Pill button** — `#cfff13` fill, `#131313` 12px semibold uppercase label, 1.44px tracking. Heights: 40 (navbar), 48 (forms)
- **Round icon button** — 40px (slider, FAQ) / 48px (social), `#cfff13` fill, fully rounded
- **Glass card / input** — 8% white fill, 1px 8% white border, 20px backdrop blur
- **Highlighted heading** — white Anton text with `#cfff13` accent word(s)
- **Feature item** — 48px icon, 24px Anton title, 16px body, centered
- **Stat item** — 72px Anton value with accent "k", 16px caption
- **FAQ item** — question row + answer, 1px white bottom border, 24px bottom padding

## Decorative patterns
None (no grid lines or dividers beyond FAQ item borders). Hero has a full-bleed photo with an empty 100×100 "Image Placeholder" frame (`1:568`) that is not visible and will not be built.

## Notes / things to flag
- Navbar button label reads **"Temlis"** in the design. It will be used verbatim.
- Benefits copy and the FAQ subtitle are identical in the design, and the footer link "Benefits" appears twice. These are used as designed.
- Hero image is oversized (1646×1097 at −136, −151) and is cropped by the 923px hero.
