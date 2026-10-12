<p align="center">
  <a href="https://www.ynot.lifestyle"><img src="assets/hero.svg" width="100%" alt="Y NOT?: streetwear storefront. Animated cover with the Y NOT? luxury streetwear lockup on cream, a charcoal hoodie printed with the oval mark swinging on a hanger, turning four-point stars, and scrolling ink and rust tickers." /></a>
</p>

<h1 align="center">Y NOT?</h1>

<p align="center"><strong>A commerce-first storefront for Y NOT?, an emerging streetwear label built around one question: why not?</strong></p>

<p align="center">
  <a href="https://www.ynot.lifestyle"><img src="assets/btn-open.svg" height="44" alt="Visit ynot.lifestyle" /></a>&nbsp;
  <a href="https://davishiggins.com"><img src="assets/btn-dh.svg" height="44" alt="Davis Higgins" /></a>
</p>

<p align="center"><sub>Live storefront · Brand system and storefront by Davis Higgins</sub></p>

---

## See it in motion

<p align="center">
  <img src="assets/demo.gif" width="880" alt="Screen recording of ynot.lifestyle: choosing the Washed Black colorway and size L for the Flame Script Hoodie, adding it to the cart, and the cart drawer opening with a free-shipping meter." />
</p>

<p align="center"><sub>Real capture of the live storefront. <a href="assets/demo.png">Static frame</a></sub></p>

## What it does

- **Shop by drop and colorway.** Collections, search, and filters lead to product pages where every colorway has its own photography and sizes are chosen per variant.
- **A cart that sells the next step.** A slide-out cart with quantity controls and a free-shipping meter hands off to a secure checkout that supports cards, Apple Pay, Google Pay, and Link.
- **Inventory that can't be oversold.** Stock is held for a shopper during checkout and released automatically if they don't finish.

## What I built

I developed the Y NOT? brand system for the web and designed and built the storefront:

- Brand application: the wordmark lockups, oval mark, star motif, cream-and-ink palette, and image treatment across every page
- Home, collection, product, search, cart, checkout, about, contact, FAQ, and policy pages
- The commerce platform behind it: pricing, payments, orders, and inventory
- Automated production setup, so every deploy arrives ready to sell
- The product photo workflow that turns raw shots into per-colorway galleries

<details>
<summary><strong>How it's put together</strong></summary>

<br />

```mermaid
flowchart TB
    C[Cart] --> P[Y NOT? commerce platform]
    P --> H[Stock held for the shopper]
    H --> S[Secure hosted checkout]
    S --> O[Order confirmed<br/>stock committed or released]
    O --> D[(Orders + inventory)]
```

| Decision | Why |
|---|---|
| **The store sets every price** | Prices, sale prices, and shipping thresholds are always decided by the store, so a modified cart can't change what someone pays. |
| **No two shoppers get the last item** | Stock is held during checkout and settled when payment completes, so inventory stays accurate under pressure. |
| **Built to handle real money safely** | Every order is recorded exactly once, even when payment updates arrive twice or out of order. |

</details>

## Screens

<table>
  <tr>
    <td width="62%"><img src="assets/screenshot-home.png" alt="Y NOT? featured collection: hoodies, a bomber jacket, and camo cargo shorts with sale prices and colorway swatches." /></td>
    <td rowspan="2" width="38%" align="center"><img src="assets/screenshot-mobile.png" width="300" alt="Y NOT? featured collection on a phone in a two-column grid." /></td>
  </tr>
  <tr>
    <td><img src="assets/screenshot-product.png" alt="Fur Hood Bomber Jacket product page with gallery, colorway swatches, sizes XS to 2XL, and details on sizing and shipping." /></td>
  </tr>
</table>

<sub>Featured collection · Product page · Collection on mobile</sub>

## Technology

| Layer | Technology |
|---|---|
| Storefront | Next.js, React, TypeScript, Tailwind CSS |
| Payments | Stripe |
| Data | Supabase |
| Motion | GSAP, Motion |
| Hosting | Vercel |

---

<p align="center">
  <a href="https://www.ynot.lifestyle"><img src="assets/btn-open.svg" height="44" alt="Visit ynot.lifestyle" /></a>&nbsp;
  <a href="https://github.com/DavisHiggins"><img src="assets/btn-more.svg" height="44" alt="More of my work" /></a>
</p>

<p align="center"><sub>© 2026 Davis Higgins. The Y NOT? name, logos, and product photography belong to Y NOT?.</sub></p>
