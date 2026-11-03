# US AIRPODS.IN

An animated product showcase website for wireless earbuds and in-ear audio devices, built with plain HTML, CSS and JavaScript.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

> **Disclaimer:** This is an educational front-end project. It is not affiliated with, endorsed by, or connected to Apple Inc. or any of the other brands whose product names appear on the page. All product names are the property of their respective owners.

---

## Overview

US AIRPODS.IN (branded "US LIFE AND INNOVATION" in the header) is a single-page product carousel. Each slide presents one pair of earbuds with a large product image, a short introduction and a "See More" button that opens a detail view with specifications and call-to-action buttons. The project focuses on CSS transitions and layered carousel animation driven by a small amount of vanilla JavaScript.

## Features

- **Layered product carousel** - six product slides arranged in depth, with each position styled through CSS custom properties (`--item1-transform` ... `--item7-transform`) for scale, blur, opacity and z-index.
- **Next / previous navigation** - the `<` and `>` buttons rotate the slide order by moving DOM nodes, with directional `next` / `prev` animations.
- **Click throttling** - navigation buttons are disabled for 2 seconds after each move so animations can finish cleanly.
- **Detail view** - "SEE MORE" switches the carousel into a `showDetail` state showing the product description, a specification grid (usage time, charging port, compatibility, Bluetooth version, controls) and "ADD TO CART" / "CHECKOUT" buttons.
- **"See All" button** - returns from the detail view to the carousel.
- **Responsive layout** - media queries at 991px and 767px adapt the layout for tablets and phones.
- **Poppins typography** loaded from Google Fonts.

Products featured on the slides: SAULT Airplugs 2X, SIMGOT EA500LM IEM, boAt Airdopes 383, JBL Live Beam 3, AirPods Pro 2 and Joi Bowie In-ear.

> Note: this is a front-end demo. The navigation links, cart and checkout buttons are visual only and are not connected to any backend or payment system, and the product descriptions use shared placeholder specification text.

## Tech Stack

| Layer | Technology |
| --- | --- |
| Markup | HTML5 |
| Styling | CSS3 (custom properties, transitions, keyframe animations, media queries) |
| Behaviour | Vanilla JavaScript (DOM manipulation, no frameworks) |
| Fonts | Google Fonts - Poppins |

## Project Structure

```
US-AIRPODS.IN/
├── index.html       # Page markup: header, carousel slides and controls
├── style.css        # Layout, carousel positions, animations, responsive rules
├── web.js           # Carousel navigation and detail-view logic
├── img1.png ... img6.png   # Product images (one per slide)
└── logo.png.webp    # Logo image (currently not referenced by the page)
```

## Getting Started

No build step or dependencies are required.

1. Clone the repository:
   ```bash
   git clone https://github.com/panchalnikhil6531/US-AIRPODS.IN.git
   cd US-AIRPODS.IN
   ```
2. Open `index.html` directly in a browser, or serve the folder locally, for example:
   ```bash
   npx serve .
   # or
   python -m http.server 8000
   ```
3. Use the `<` and `>` buttons to browse products and **SEE MORE** to open the detail view.

## Author

**Panchal Nikhil S**

- GitHub: [@panchalnikhil6531](https://github.com/panchalnikhil6531)
- LinkedIn: [nikhil-s-panchal](https://www.linkedin.com/in/nikhil-s-panchal-463a78319/)
- Portfolio: [potfolio-beta-two.vercel.app](https://potfolio-beta-two.vercel.app/)
