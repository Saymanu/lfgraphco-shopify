# L F Graphco Launch Checklist

Review date: 2026-06-10

This checklist is based on a repository-wide deployment readiness review of the Shopify theme files, with extra attention on `docs/`, `templates/`, `sections/`, `snippets/`, `layout/`, `config/`, storefront assets, brand source files and the pricing reference.

## Review summary

The theme is close to launch as a quote-first Shopify storefront. It includes a homepage, service pages, local SEO pages, collection templates, product/cart/blog templates, quote/contact/artwork forms, starting-price sections, local optimized photo assets, brand logo assets, structured data, mobile CTA, exit-intent lead capture and tracking placeholders.

The remaining launch risk is mostly outside the repository: Shopify Admin setup, live page handle assignment, products and collections, policy/checkout/shipping/tax settings, tracking account IDs, conversion event QA, Merchant Center feed setup and advertising account readiness.

## Reviewed areas

- Existing documentation in `docs/`
- Homepage, service page, local SEO page and conversion landing templates
- Product, collection, cart and blog templates
- Quote, contact, upload artwork, lead capture and exit-intent forms
- Pricing sections and `brand-assets/pricing/LFGraphco_Pricing_Reference.md`
- Header, footer, mobile CTA and internal `/pages/...` and `/collections/...` links
- Local photo assets, logo assets, favicon and brand color settings
- SEO metadata, canonical tag, Open Graph/Twitter metadata and LocalBusiness structured data
- Tracking snippets for GA4, GTM, Meta Pixel, Klaviyo and Google Ads
- Shopify theme settings in `config/settings_schema.json` and `config/settings_data.json`

## Phase 1 - Required before website launch

### 1. Upload and preview the theme in Shopify

- Description: Upload the repository as a Shopify Online Store 2.0 theme, preview every major template and confirm the storefront renders correctly on desktop and mobile.
- Priority: Critical
- Estimated time: 1-2 hours
- Owner: Requires user action in Shopify Admin; Codex can support with theme file fixes if preview issues appear.

### 2. Create Shopify pages with matching handles

- Description: Create Shopify pages and assign the matching templates for About, Screen Printing, Embroidery, DTF Printing, Promotional Products, Team Stores, School Spirit Wear, Company Uniforms, Church Apparel, Fundraising, Contact, Request A Quote, Upload Artwork, FAQ and local SEO pages.
- Priority: Critical
- Estimated time: 1.5-3 hours
- Owner: Requires user action in Shopify Admin; Codex can provide a handle/template mapping.

### 3. Verify all header, footer, CTA and internal links

- Description: Confirm every `/pages/...` and `/collections/...` link resolves in the live Shopify preview after pages and collections are created.
- Priority: Critical
- Estimated time: 45-90 minutes
- Owner: Requires user action for live Shopify preview access; Codex can audit theme references and fix repo-level links.

### 4. Test all Shopify contact forms

- Description: Submit test leads through Contact, Request A Quote, Upload Artwork, homepage lead capture and exit-intent popup forms, then confirm notification delivery and captured fields.
- Priority: Critical
- Estimated time: 1-2 hours
- Owner: Requires user action in the live Shopify store and email inbox; Codex can adjust form fields or labels in theme files.

### 5. Decide the artwork intake workflow

- Description: The current theme collects an artwork file link because native Shopify contact forms do not upload files directly. Decide whether that is acceptable for launch or whether to connect a dedicated file-upload app/workflow.
- Priority: Critical
- Estimated time: 30-60 minutes for decision; 2-4 hours if implementing an app workflow.
- Owner: Requires user action for app/account selection; Codex can update copy and theme fields.

### 6. Add store policies and legal pages

- Description: Configure refund, privacy, terms of service, shipping and contact/legal policy pages in Shopify Admin, then link them in footer or checkout as needed.
- Priority: Critical
- Estimated time: 1-3 hours
- Owner: Requires user action for business/legal approval; Codex can draft non-legal starter copy for review.

### 7. Configure checkout, payments, taxes and shipping

- Description: Confirm Shopify payments, tax settings, local delivery/pickup or shipping profiles, checkout branding and notification emails before accepting orders.
- Priority: Critical
- Estimated time: 2-4 hours
- Owner: Requires user action in Shopify Admin and payment/tax accounts.

### 8. Create required collections

- Description: Create collections for Custom T-Shirts, Embroidered Polos, Hoodies, Safety Apparel, Company Uniforms, Spirit Wear, DTF Transfers and Promotional Products so collection links and category cards resolve.
- Priority: Critical
- Estimated time: 1-2 hours
- Owner: Requires user action in Shopify Admin; Codex can provide collection naming and SEO suggestions.

### 9. Add initial products or intentionally launch quote-only

- Description: Product and collection templates are present, but real Shopify products, variants, media, inventory/pricing and collection assignments must be added if ecommerce sales are part of launch. If launching quote-only, hide empty shop navigation or keep empty collection CTAs intentional.
- Priority: High
- Estimated time: 4-12 hours depending on product count
- Owner: Requires user action for product data, pricing approval and Shopify Admin entry; Codex can create product copy and CSV drafts.

### 10. Add real product photography or mockups

- Description: The theme has optimized shop/customer photos, but product pages still depend on Shopify product media. Add product-specific images for purchasable products and clear mockups for quote packages.
- Priority: High
- Estimated time: 2-8 hours
- Owner: Requires user action for photos/mockups; Codex can help resize, name and document assets.

### 11. Confirm pricing and margin approval

- Description: Review all starting prices from the pricing reference and storefront sections, including t-shirts, hoodies, polos, DTF transfers and promotional products, before publishing.
- Priority: High
- Estimated time: 1-2 hours
- Owner: Requires user action for business approval; Codex can update pricing copy if numbers change.

### 12. Finalize business identity details

- Description: Confirm phone number, business name, service area, address visibility, email recipients and footer/contact details are accurate.
- Priority: High
- Estimated time: 30-60 minutes
- Owner: Requires user action; Codex can update theme settings defaults or copy.

### 13. Configure page SEO titles and meta descriptions in Shopify

- Description: The theme has fallback metadata, but each live page should have a custom Shopify SEO title and meta description for launch.
- Priority: High
- Estimated time: 2-4 hours
- Owner: Requires user action in Shopify Admin; Codex can draft titles and descriptions.

### 14. Confirm brand rendering

- Description: Check logo, favicon, brand colors, header, footer, hero and mobile CTA against L F Graphco branding in the live theme preview.
- Priority: High
- Estimated time: 30-60 minutes
- Owner: Requires user action for visual approval; Codex can adjust assets/CSS.

### 15. Mobile usability QA

- Description: Test the sticky header, horizontally scrollable navigation, mobile CTA, forms, pricing tables, galleries and popup on common mobile viewport sizes.
- Priority: High
- Estimated time: 1-2 hours
- Owner: Codex can complete repo/browser QA if a preview URL is available; user action may be needed for Shopify preview access.

### 16. Accessibility smoke test

- Description: Confirm keyboard navigation, visible focus, form labels, alt text, popup close behavior, skip link and color contrast in the live preview.
- Priority: Medium
- Estimated time: 1-2 hours
- Owner: Codex can complete most checks with browser access; user action may be needed for final acceptance.

### 17. Publish navigation menus in Shopify Admin

- Description: Build or adjust Shopify navigation menus to match the theme's service, quote, upload artwork and collection paths.
- Priority: Medium
- Estimated time: 45-90 minutes
- Owner: Requires user action in Shopify Admin; Codex can provide a recommended menu structure.

### 18. Add blog content or hide blog links

- Description: The blog template exists, but blog articles need to be created if blog links will be public. Otherwise, keep blog out of launch navigation.
- Priority: Medium
- Estimated time: 1-4 hours for initial posts
- Owner: Requires user action for publishing; Codex can draft article outlines or starter posts.

## Phase 2 - Required before running Google Ads

### 1. Create and connect GA4

- Description: Create a Google Analytics 4 property, add the Measurement ID to theme settings and confirm page_view collection.
- Priority: Critical
- Estimated time: 45-90 minutes
- Owner: Requires user action for Google account access; Codex can verify snippet behavior after the ID is entered.

### 2. Create and connect Google Tag Manager

- Description: Create a GTM container, add the container ID to theme settings and use GTM as the main routing layer for ad and conversion tags.
- Priority: Critical
- Estimated time: 1-2 hours
- Owner: Requires user action for GTM account access; Codex can advise on events and theme data hooks.

### 3. Configure Google Ads account and conversion actions

- Description: Create Google Ads conversion actions for quote leads, contact leads, artwork submissions, phone calls and purchases if checkout is active.
- Priority: Critical
- Estimated time: 1-3 hours
- Owner: Requires user action in Google Ads; Codex can document event names and recommended triggers.

### 4. Implement and test form conversion events

- Description: Track successful submissions for quote, contact, artwork, lead capture and popup forms. Shopify contact form success states should be validated in the live store.
- Priority: Critical
- Estimated time: 2-4 hours
- Owner: Requires user action for live testing and account access; Codex can update theme snippets or GTM guidance.

### 5. Configure phone-call tracking

- Description: Track clicks on phone links and decide whether to use Google forwarding numbers, call extensions/assets or a call tracking provider.
- Priority: Critical
- Estimated time: 1-2 hours
- Owner: Requires user action in Google Ads or call tracking platform; Codex can add consistent event hooks if needed.

### 6. Set up Google Search Console

- Description: Verify the domain, submit sitemap and check indexing coverage before paid traffic starts.
- Priority: High
- Estimated time: 30-60 minutes
- Owner: Requires user action for domain/Google access.

### 7. Prepare landing page SEO and ad-message consistency

- Description: Confirm ad groups map to relevant pages such as Screen Printing, Embroidery, DTF Printing, Promotional Products, Team Stores and local pages.
- Priority: High
- Estimated time: 1-3 hours
- Owner: Codex can draft mapping and page copy updates; user action required for final campaign approval.

### 8. Confirm no misleading claims in ad landing pages

- Description: DTF and promotional product pages correctly avoid claiming unsupported machine/product photos. Recheck all ad landing pages for accurate service, price and turnaround claims.
- Priority: High
- Estimated time: 45-90 minutes
- Owner: Codex can audit copy; user action required for business approval.

### 9. Add privacy/cookie disclosures required by tracking setup

- Description: Update privacy/cookie policy language to disclose analytics, advertising pixels, email marketing and retargeting.
- Priority: High
- Estimated time: 1-2 hours
- Owner: Requires user/legal approval; Codex can draft starter policy language for review.

### 10. Configure Meta Pixel if retargeting will run

- Description: Add Meta Pixel ID to theme settings or connect via Shopify sales channel, then confirm PageView and lead events as needed.
- Priority: Medium
- Estimated time: 1-2 hours
- Owner: Requires user action for Meta account access; Codex can verify theme rendering.

### 11. Configure Klaviyo before email capture campaigns

- Description: Add Klaviyo Company ID and confirm Shopify integration, consent settings and lead follow-up flows.
- Priority: Medium
- Estimated time: 1-3 hours
- Owner: Requires user action in Klaviyo and Shopify; Codex can help with form copy and flow outlines.

### 12. Create ad-ready thank-you or confirmation flow

- Description: Shopify contact forms show inline success messages, but ads benefit from a clear conversion confirmation path or event trigger strategy.
- Priority: Medium
- Estimated time: 2-4 hours
- Owner: Codex can implement theme changes if the desired flow is chosen; user action required for approval/testing.

## Phase 3 - Required before scaling advertising

### 1. Complete Google Merchant Center setup

- Description: Verify and claim the domain, connect Shopify products, submit feed data and resolve diagnostics before Shopping or Performance Max scaling.
- Priority: Critical
- Estimated time: 3-8 hours
- Owner: Requires user action in Merchant Center and Shopify; Codex can help with product feed copy and diagnostics interpretation.

### 2. Build complete product catalog data

- Description: Add product titles, descriptions, images, pricing, variants, availability, shipping attributes, tax settings and collection assignments for feed-ready products.
- Priority: Critical
- Estimated time: 8-24 hours depending on catalog size
- Owner: Requires user action for product data and Shopify Admin work; Codex can generate CSV/product copy drafts.

### 3. Validate conversion tracking end to end

- Description: Confirm GA4, GTM, Google Ads, Meta and Shopify reporting agree on lead and purchase activity before increasing budgets.
- Priority: Critical
- Estimated time: 2-6 hours
- Owner: Requires user action/account access; Codex can audit tags and theme implementation.

### 4. Add dedicated campaign landing pages if needed

- Description: Build narrower landing pages for high-intent ads such as "screen printing Garland TX", "custom t-shirts Dallas", "embroidered polos", "team stores" and "booster club shirts".
- Priority: High
- Estimated time: 2-6 hours per page
- Owner: Codex can create templates/copy; user action required for approval and Shopify page creation.

### 5. Improve mobile navigation for paid traffic

- Description: The current mobile header uses horizontal scrolling for many links. Consider a collapsible menu if paid traffic shows navigation friction.
- Priority: High
- Estimated time: 3-6 hours
- Owner: Codex can implement; user action required for visual approval.

### 6. Add stronger lead qualification and routing

- Description: Extend forms or follow-up workflows to capture budget, garment type, decoration locations, deadline urgency and preferred contact method.
- Priority: High
- Estimated time: 2-5 hours
- Owner: Codex can update theme forms; user action required for sales workflow decisions.

### 7. Add review/testimonial proof

- Description: Add customer testimonials, logos, project stories or review embeds to improve paid traffic trust.
- Priority: High
- Estimated time: 2-6 hours
- Owner: Requires user action to provide approved testimonials; Codex can create sections and layout.

### 8. Add campaign-specific photography and mockups

- Description: Add more service-specific visuals for promo products, DTF transfers, team stores and corporate apparel to reduce reliance on general apparel photos.
- Priority: Medium
- Estimated time: 4-12 hours
- Owner: Requires user action for photo/mockup sourcing; Codex can optimize and integrate assets.

### 9. Create email/SMS lead follow-up flows

- Description: Build automated follow-up for quote requests, artwork reminders, abandoned carts and returning customers.
- Priority: Medium
- Estimated time: 4-10 hours
- Owner: Requires user action in Klaviyo/SMS tools; Codex can draft copy and implementation guidance.

### 10. Add reporting dashboard conventions

- Description: Define weekly reporting for spend, leads, cost per lead, quote quality, close rate, revenue and top landing pages.
- Priority: Medium
- Estimated time: 2-4 hours
- Owner: Requires user action for business metrics; Codex can create a reporting template.

### 11. Improve schema coverage

- Description: Add product, FAQ or service-specific structured data where appropriate once live products and final FAQs exist.
- Priority: Medium
- Estimated time: 2-5 hours
- Owner: Codex can implement after final content/products are available.

## Phase 4 - Future enhancements

### 1. Build a true file upload flow

- Description: Replace artwork link fields with a direct upload workflow using a Shopify app, customer account upload path or external upload service.
- Priority: Medium
- Estimated time: 4-10 hours
- Owner: Requires user action for app/service choice; Codex can integrate theme copy and links.

### 2. Add a quote configurator

- Description: Create guided quote steps for garment type, quantity, print locations, colors, deadline and artwork status.
- Priority: Medium
- Estimated time: 8-20 hours
- Owner: Codex can implement theme-side UI; user action required for pricing/business rules.

### 3. Add team store launch templates

- Description: Build reusable page/product patterns for schools, teams, churches and companies launching temporary stores.
- Priority: Medium
- Estimated time: 6-16 hours
- Owner: Codex can create templates; user action required for operational workflow.

### 4. Add more localized SEO pages

- Description: Expand beyond Garland, Mesquite, Dallas and DFW into nearby service areas once core pages are indexed and performing.
- Priority: Medium
- Estimated time: 1-3 hours per page
- Owner: Codex can draft and create templates; user action required for location/service approval.

### 5. Add case studies and project galleries

- Description: Publish project pages showing finished apparel, customer goals, production method and results.
- Priority: Medium
- Estimated time: 2-5 hours per case study
- Owner: Requires user action for customer approval/photos; Codex can draft and structure pages.

### 6. Add advanced ecommerce merchandising

- Description: Improve product filters, size charts, bulk order messaging, related products and collection merchandising as the catalog grows.
- Priority: Low
- Estimated time: 6-20 hours
- Owner: Codex can implement theme improvements after catalog data exists.

### 7. Add A/B testing plan

- Description: Test hero messaging, CTA wording, form length, pricing placement and lead magnet offers once traffic volume is high enough.
- Priority: Low
- Estimated time: 4-12 hours
- Owner: Requires user action for testing platform/budget decisions; Codex can create variants.

### 8. Add richer accessibility testing

- Description: Run a full accessibility review with automated checks and manual keyboard/screen reader testing after the live Shopify theme is stable.
- Priority: Low
- Estimated time: 4-8 hours
- Owner: Codex can perform automated and manual checks with site access; user action required for final acceptance.

### 9. Add performance optimization pass

- Description: Review image sizes, CSS duplication, app impact, third-party scripts and Core Web Vitals after Shopify apps and tracking are installed.
- Priority: Low
- Estimated time: 3-8 hours
- Owner: Codex can audit and optimize repo-level assets; user action may be required for Shopify app decisions.

### 10. Add CRM or pipeline integration

- Description: Route quote requests into a CRM, spreadsheet or sales pipeline so leads are tracked from request to close.
- Priority: Low
- Estimated time: 4-12 hours
- Owner: Requires user action for CRM/tool choice; Codex can help with integration planning and copy.

## Launch decision

Do not publish the site until Phase 1 critical items are complete. Do not run Google Ads until Phase 2 critical items are complete and conversion tracking has been tested. Do not scale advertising until Phase 3 critical items are complete and lead quality can be measured reliably.
