# Desert Bloom Foundation

**Where grocery stores don't reach, Desert Bloom does.**

The official website for Desert Bloom Foundation — a youth-led 501(c)(3) nonprofit
based in Harrison, New York, bringing fresh, hand-chosen meals to neighbors across
Westchester's food deserts. Founded and run by twin brothers Daniel and Liam Wellisch,
in partnership with local corporate sponsors, farms, and kitchens (including CSA Kitchen
in Mount Vernon, the largest food desert we serve).

## Viewing the site

No build step, no dependencies, no framework install. Either:

- Open **`index.html`** in any modern browser, or
- Open **`Desert Bloom Foundation.dc.html`** directly, or
- Serve the folder and visit it, e.g.:

  ```bash
  python3 -m http.server 8000
  # then open http://localhost:8000
  ```

The page is fully responsive (desktop + mobile), and all content is visible without
JavaScript — the motion and interactions are progressive enhancements.

## Project structure

```
index.html                     Redirect entry point (for GitHub Pages / quick open)
Desert Bloom Foundation.dc.html The site (a self-contained Design Component)
support.js                     The runtime that renders the Design Component
assets/
  logo-mark.png  logo-full.png Brand logo (palette source)
  founder-*.png                Founder portraits
  partner-*.png                Partner marks
  photos/                      Optimized event & kitchen photography (p*.jpg, g*.jpg)
uploads/                       Original, full-resolution source photos
```

## Forms

The **Partner** and **Volunteer** forms submit in the background via
[Formspree](https://formspree.io) and email the details to the foundation, copying the
sender. The two endpoints live in the logic class (`FORM_ENDPOINT`):

- Partner: `https://formspree.io/f/xvzjadqg`
- Volunteer: `https://formspree.io/f/xqevqwdg`

If an endpoint is unconfirmed or unreachable, the form falls back to opening a
pre-addressed email draft to `desertsbloomfoundation@gmail.com`. Confirm each form once
in the Formspree dashboard to activate background sending.

## Donate

Donations go through GoFundMe: https://gofund.me/7fcaa4515

## Contact

- Email: desertsbloomfoundation@gmail.com
- Instagram: [@desertbloomfoundation](https://instagram.com/desertbloomfoundation)

---

© Desert Bloom Foundation. Photography and brand assets are property of the foundation.
