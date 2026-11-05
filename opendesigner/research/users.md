# Kat: who the users are

> Desk research by an AI agent with OpenDesigner, from public sources it opened. It describes a group, not this product's own users: confirm what matters with real people (five short interviews are enough to start). Rendered from `users.json`; edit that file and run `engine.py research add` again.

**Users:** Người đặt đồ ăn vặt và thức uống ở Việt Nam, chủ yếu thao tác trên điện thoại; có thể là khách vãng lai, khách đăng nhập hoặc nhân viên admin.

**Researched:** 2026-11-04

**Tools used:** web-search, browser

**Not available:** last30days, mobbin, deep-research, analytics

## Findings

### Who they are

- **F1** In PwC's 2025 Vietnam sample of 517 consumers, 58% bought prepared food at least weekly and 54% ordered takeaway to their home; the study does not describe Kat's own customers. (measured; [S1])

### Where and how they use it

- **F2** Decision Lab reported that 65% of eligible residents in Hanoi, Ho Chi Minh City and Da Nang had ordered from a food-delivery app in the past month, using 1.7 apps on average. (measured; [S2])
- **F8** A 2024 Vietnam Internet Index cited 78.44 million internet users and 3.5 hours of daily mobile internet use; it is broad digital context and does not establish food-ordering behavior. (measured; [S3])

### The apps they already use every day, and the patterns those apps have taught them

- **F3** Decision Lab's 2025 market study identifies ShopeeFood and GrabFood as the two largest food-delivery alternatives in its surveyed market; this is a market signal, not a measure of Kat customer preferences. (measured; [S2])

### What they expect and what frustrates them

- **F4** Baymard's US e-commerce research reports extra costs and forced account creation among checkout friction points; its percentages are not Vietnam estimates, but the findings support clear fees and a visible guest path. (measured; [S4], [S5])

### Preferences that touch design

- **F5** PwC's 2025 Vietnam survey says price remains a primary food-purchase driver, so showing item prices, delivery fees and voucher savings together may help people judge value; this is a design inference. (inferred; [S1])

### Access needs common in the group

- **F6** WCAG 2.2 AA sets a 24 by 24 CSS pixel minimum for pointer targets in most cases; this is a general accessibility floor, not a Vietnam-specific user finding. (reported; [S6])

### The market

- **F7** Grab says food-delivery ETAs depend on distance, time of day and external conditions, so a local demo without live logistics should not promise a precise delivery time. (reported; [S7])

## Apps they already use

- **ShopeeFood**: A leading alternative in the 2025 Vietnam food-delivery market study. ([S2])
- **GrabFood**: A leading alternative in the 2025 Vietnam food-delivery market study; its published terms explain why delivery estimates vary. ([S2], [S7])

## Patterns they already know

- Make guest ordering easy to spot and do not require registration before checkout.
- Show delivery and item costs before the final order action.
- Treat any delivery-time display as an estimate tied to real logistics data.

## Market

- **Analogous product:** Popeyes ordering flow: The handoff names it as an ordering-experience reference; its brand identity is not part of this research or design. [S8]
- **Competitors:** ShopeeFood: A leading food-delivery alternative in the 2025 market study. [S2]; GrabFood: A leading food-delivery alternative in the 2025 market study. [S2]; Ordering directly from Kat: The project brief describes a single-restaurant ordering site. [S8]
- **What they all do:** Urban customers use several food-delivery apps, and delivery estimates depend on order context. [S2, S7]
- **The gap:** This short desk review did not identify a reliable unmet market need; validate any differentiation with Kat customers.
- **Conventions:** Vietnamese đồng price labels; Delivery or pickup choice; Guest order path; Visible order total

## What it means for the design system

- Already the answer: Q-aud-01 = **Now and then, on a phone or in public** (from F8; signals occasional-mobile)
- Applied: Q-aud-02 = **consumer** (from F1, F2, F4; the user approved applying this choice to PRODUCT.md)
- For later stages: Follow the patterns of the apps they live in before inventing new ones (practices.md sections 2 and 3). (from F2, F3)

## Open questions

- What ages, neighborhoods and devices do Kat's own customers use?
- Which product photos, wording and price/value cues best fit Kat's real menu?
- Do Kat customers want pickup availability or delivery estimates beyond the fixed demo rules in the handoff?

## Sources

- [S1] [Voice of the Consumer Survey 2025 - Vietnam Snapshot](https://www.pwc.com/vn/en/publications/2025/voice-of-consumer-2025.pdf) · survey, published 2025, opened 2026-11-04
- [S2] [Racing ahead in Vietnam's competitive food delivery landscape](https://www.decisionlab.co/racing-ahead-vietnams-competitive-food-delivery-landscape) · study, published 2025, opened 2026-11-04
- [S3] [Vietnam Innovation & Tech Investment Report 2024 - Vietnam Internet Index](https://nic.gov.vn/img/wpuploads/2024/05/Vietnam-Innovation-Tech-Investment-Report-2024_ENG.pdf) · official-stats, published 2024, opened 2026-11-04
- [S4] [Make Guest Checkout the Most Prominent Option](https://baymard.com/research-articles/make-guest-checkout-prominent) · study, published 2023-01-17, opened 2026-11-04
- [S5] [50 Cart Abandonment Rate Statistics 2026](https://baymard.com/lists/cart-abandonment-rate?goal=scale-support) · study, published 2026, opened 2026-11-04
- [S6] [Understanding Success Criterion 2.5.8: Target Size (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum) · article, opened 2026-11-04
- [S7] [Terms of Service: Transport, Delivery and Logistics - Grab Vietnam](https://www.grab.com/vn/terms-policies/transport-delivery-logistics/) · article, published 2026, opened 2026-11-04
- [S8] Project handoff brief: Maika and Popeyes ordering-flow inspiration (person, 2026-11-04) · person, published 2026-11-04, opened 2026-11-04
