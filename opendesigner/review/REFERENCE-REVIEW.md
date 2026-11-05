# Reference review: Maika and Popeyes

Reviewed 2026-11-04 for Kat's snack-ordering website. Maika and Popeyes are experience references. Kat is the project brand; another restaurant's logo, colors, imagery, copy, contact details, branches or offers are not used as Kat content.

## Maika

Pages reviewed: [home](https://quananmaika.com/), [menu collection](https://quananmaika.com/collections/thuc-don), [menu page](https://quananmaika.com/pages/menu), [about](https://quananmaika.com/pages/about-us), [contact and feedback](https://quananmaika.com/pages/lien-he), and [careers](https://quananmaika.com/pages/tuyen-dung).

- The home page puts contact details, menu categories, the Asian-with-Vietnamese-flavor story, opening information, signature dishes, reviews, offers, and branches into one long storefront. The main menu also exposes filters, prices, sorting, and add-to-cart actions.
- The live menu currently lists 81 products and nine categories. Kat's demo keeps its ten sample snack products rather than copying the live catalog or inventing the missing items.
- The live home page lists 528–530 Nguyễn Trãi and 155 Nguyễn Đình Chiểu, and says 10:00–22:00. Other live pages conflict: the contact page lists a different Quận 5 address and 9:00–22:00, while the home and menu pages contain both 15- and 30-minute delivery claims. Kat uses editable placeholders for branches and hours and makes no delivery-time promise.
- The live offer still advertises a code with an expiry date of 10/10/2024. That old offer is not reused. Kat displays only its own demo voucher data.
- The review area on the live home page uses testimonials. Kat has no verified customer testimonials, so the rebuilt home page uses locally stored product reviews and an honest empty state.
- Careers content includes role, wage, age and shift details that can change. Kat does not copy them.

## Popeyes Vietnam

The official [policy page](https://popeyes.vn/policy) was readable and exposes the main navigation: promotions, menu, stores, order tracking and catering. Direct requests to the Popeyes home, promotion and category pages returned HTTP 403 in the research tool. The attached user walkthrough is therefore treated as owner-supplied observation for those pages, not as an independently verified current render.

Useful patterns for Kat are early delivery or pickup intent, a visible path into deals and menu, persistent cart access, and order tracking. Kat adapts those patterns to its snack catalog and localStorage checkout. It does not claim Popeyes discounts, prices, delivery times or inventory.

## Scope limits

This was a content and navigation review, not a computed-style or interaction capture. Popeyes' blocked pages were not bypassed. The Maika pages supplied text and navigation but not reliable motion, hover states or a fresh rendered comparison at Kat's viewport sizes. See `AUDIT.md` and `REPORT.md` for the code review and visual review limits.
