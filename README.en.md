# House direction check

Property browsers check on the spot whether a house faces a direction that suits them.

*[Đọc bản tiếng Việt](README.md)*

**See it running:** https://nhatnguyet.org/widget/huong-nha

## Paste these two lines

```html
<div data-widget="huong-nha"></div>
<script async src="https://nhatnguyet.org/embed/w.js"></script>
```

No account, no API key, nothing to pay.

## What it gives your page

For property and interiors sites: a visitor looking at one particular house checks whether its facing suits their birth year without leaving the listing. If you already know which way the house faces, set it through data-huong and the visitor only picks a year.

## Worth knowing before you embed

- If you already know which way the house faces, pin it, and the visitor only picks a birth year while the answer speaks about the house in front of them.
- Bat Trach is one school of feng shui among several, and the table uses the solar year as an approximation of the lunar one. The widget says both.
- An unsuitable direction is shown in amber, not red. This is folk belief about a house, not a safety warning.

## The steps

1. Paste the snippet into the listing detail page.
2. If you know the facing, add data-huong, for example dong-nam, to save the visitor a step.
3. If you do not, leave it out and the visitor picks from an eight-point compass.

## Where to paste it

**WordPress.** Add a *Custom HTML* block to the post, or a *Text* widget in
the sidebar, and paste both lines there. Do not paste into the ordinary
editor: it will show the code as text instead of running it.

**Wix, Squarespace, Shopify.** Use the *Embed HTML* / *Custom HTML* block.

**Hand-written sites.** Paste it straight where you want the widget. If you
embed several widgets, the `<script>` line only needs to appear once on the
page.

**A note on width.** The widget fits the width of wherever you put it. If that is narrower than 280px, add
`data-size="compact"`; if it is a wide horizontal strip, use
`data-size="wide"`.

## Make it match your page

| Attribute | Values | Meaning |
|---|---|---|
| `data-widget` | `huong-nha` | Required |
| `data-theme` | light or dark | Defaults to light |
| `data-accent` | #b3341f | Accent colour as a 6-digit hex value, to match your own branding |
| `data-lang` | vi or en | Defaults to vi |
| `data-size` | compact, standard or wide | Level of detail for the width you have: compact drops secondary detail, wide lays out horizontally. Defaults to standard |
| `data-huong` | dong-nam, tay-bac... | Pin the house facing for the direction widget, so the visitor only picks a birth year |

With every attribute this widget accepts, it looks like this:

```html
<div data-widget="huong-nha" data-theme="dark" data-accent="#1f6f5c" data-lang="en" data-size="compact" data-huong="dong-nam"></div>
<script async src="https://nhatnguyet.org/embed/w.js"></script>
```

Want to see it for yourself before it goes near your real page? Open
[`vi-du/index.html`](vi-du/index.html) in a browser, nothing to install.

## A few things we ask

- Free for personal and business websites, with no display limit.
- Keep the attribution line at the foot of the widget. That is what you give
  in return for free use.
- Do not embed on gambling, adult, fraudulent sites or anything unlawful
  under Vietnamese law.
- The content is folk knowledge and cultural convention, offered as
  reference, not as health, financial or legal advice.

Full text: [`TERMS.md`](TERMS.md) · [https://nhatnguyet.org/widget/dieu-khoan](https://nhatnguyet.org/widget/dieu-khoan)

## Who we are

Nhat Nguyet (https://nhatnguyet.org) is a Vietnamese reference site for calendrical and
cultural knowledge: the lunar calendar computed for Vietnam's own time zone,
the sexagenary cycle, solar terms, auspicious hours, astrology, feng shui,
and a glossary of terms.

There is one thing we try hard to keep clear, even inside a 300px frame:
which parts are computed, and which are folk convention.

Lunar dates, sexagenary names and solar terms are **computed**. Run the same
calculation and you get the same answer, and we publish the underlying
datasets under CC BY 4.0 so you can check for yourself.

Auspicious hours, Bat Trach directions and Lo Ban rule bands are **cultural
convention**. There are real lookup tables behind them, but they are not
measurements. The widget tells you what the table says; how much weight to
give it is yours to decide.

Where the schools disagree, we say so, rather than quietly picking a side and
presenting it as the only reading.

Open data: [GitHub](https://github.com/taman-spirit/du-lieu-am-lich) ·
[Hugging Face](https://huggingface.co/datasets/nhatnguyet)

## Something not right?

Open an issue in this repository. We do read them.

The whole widget library: [https://nhatnguyet.org/widget](https://nhatnguyet.org/widget)
