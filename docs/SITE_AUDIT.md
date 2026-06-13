# Site Audit

Audit date: 2026-06-10

## What Was Checked

- Theme templates in `templates/`
- Reusable Shopify sections in `sections/`
- Snippets, layout, tracking placeholders and structured data
- Header, footer, homepage, service pages, quote forms, upload artwork, collections, product, blog and cart templates
- Internal `/pages/...` links referenced by theme files
- Image references, alt text, file formats and missing image fallbacks
- Lead forms, quote calls-to-action, mobile sticky CTA and exit-intent popup
- Mobile layout CSS for grids, forms, photo sections and CTA bars
- SEO basics including titles, meta fallback, canonical tag, Open Graph/Twitter tags and LocalBusiness structured data
- Accessibility basics including labels, alt text, skip link, form autocomplete and popup focus behavior

## Punch List

### Fixed Automatically

- Replaced raw GitHub image URLs and HEIC storefront image references with optimized local theme assets.
- Replaced the product image fallback text that said "placeholder" with conversion-focused quote and artwork copy.
- Added an artwork file link field to the quote and upload artwork forms.
- Added autocomplete attributes to contact, quote, upload artwork, homepage lead capture and popup form fields.
- Improved exit-intent popup behavior by focusing the first interactive field when the popup opens.
- Fixed the homepage services grid so full-color apparel production does not distract from the core custom service path.
- Improved empty collection messaging with a direct Request A Quote CTA.
- Updated deployment documentation to remove outdated placeholder-branding language and include the new conversion landing templates.
- Updated photo documentation to clarify that storefront sections use optimized JPG assets rather than direct HEIC originals.

### Issues Found

- Missing images: product pages still depend on Shopify product media. The theme now has a stronger fallback, but real product images must be added in Shopify Admin.
- Placeholder text: no customer-facing placeholder branding remains in theme sections. Tracking placeholders remain intentionally documented because IDs are not available yet.
- Broken links: static theme links to `/pages/...` all have matching page templates. Shopify Admin still needs pages created with matching handles.
- Empty sections: collections and blog can be empty until products/articles are created. Empty collection messaging now drives quote requests.
- Duplicate content: some service and landing page messaging intentionally overlaps around quote requests, but no exact duplicate page templates were found that require automated removal.
- Mobile usability: grids and forms collapse responsively. The header navigation may become horizontally scrollable on smaller screens because it contains many service links.
- SEO: fallback metadata, canonical URLs, social tags and LocalBusiness structured data are present. Final page-specific SEO titles/descriptions should be configured in Shopify Admin.
- Accessibility: form labels, alt text and skip link are present. Popup focus behavior was improved. Full keyboard/focus trapping should be tested in a live browser preview.
- Conversion: primary quote paths are strong. Product, collection and upload flows were improved with additional quote/artwork CTAs.
- Missing calls-to-action: fixed on empty collection and product fallback states. Remaining CTAs depend on live products and policy pages.

## Remaining Items Requiring User Input

- Create Shopify pages using the matching templates and handles used by the header/footer links, including Shop Collections and Banners and Signs.
- Add real Shopify products, product images, variants, prices, personalization options and collection assignments.
- Add blog articles if the blog template will be linked publicly.
- Add final SEO titles and meta descriptions in Shopify Admin for every live page.
- Enter real Google Analytics, Google Tag Manager, Meta Pixel, Klaviyo and Google Ads IDs when accounts are ready.
- Decide whether the header navigation should remain horizontally scrollable on mobile or move to a collapsible menu.
- Connect a true file upload workflow if customers need direct file attachment instead of an artwork link field.
- Add store policies, shipping, tax, checkout and legal pages before launch.
