# Shopify Deployment Guide

## Theme deployment

1. Create or open the L F Graphco LLC Shopify store.
2. Install Shopify CLI locally and authenticate with the store.
3. Upload this repository as an Online Store 2.0 theme.
4. In Shopify Admin, create pages that use these templates:
   - About Us: `page.about`
   - Screen Printing: `page.screen-printing`
   - Embroidery: `page.embroidery`
   - Full-Color Apparel Printing: `page.dtf-printing`
   - Promotional Products: `page.promotional-products`
   - Team Stores: `page.team-stores`
   - School Spirit Wear: `page.school-spirit-wear`
   - Company Uniforms: `page.company-uniforms`
   - Church Apparel: `page.church-apparel`
   - Banners and Signs: `page.banners-signs`
   - Shop Collections: `page.shop-collections`
   - Fundraising: `page.fundraising`
   - Fundraiser: `page.fundraiser`
   - Contact: `page.contact`
   - Request A Quote: `page.request-a-quote`
   - Upload Artwork: `page.upload-artwork`
   - FAQ: `page.faq`
   - Family Reunion Shirt Sale: `page.family-reunion-shirts-sale`
5. Create local SEO pages using the matching page templates for Garland, Mesquite, Dallas and DFW search targets.
6. Configure navigation links to match the header and footer paths.

## Product setup

Create Shopify collections for Custom T-Shirts, Embroidered Polos, Hoodies, Safety Apparel, Company Uniforms, Spirit Wear, Banners and Signs, Promotional Products and the five retail shop collections. Use clear product titles, size variants, color variants, personalization properties, pricing, images and collection assignments. Birthday and Family Event Shirts can remain a future collection, but Teacher Shirts should be the active school-friendly retail launch focus.

Retail collection handles:

- `bridal-party-shirts`
- `grandma-nana-mimi-shirts`
- `sports-mom-shirts`
- `teacher-shirts`
- `texas-pride-shirts`

The first retail product launch package lives in `marketing/shopify-retail-products-launch.csv` with supporting notes in `docs/RETAIL_PRODUCT_LAUNCH_PACKAGE.md`.

## Launch checklist

- Confirm logo, favicon and extracted L F Graphco colors render correctly in the live theme preview.
- Add product photograpy or apparel mockups.
- Add retail products with size, shirt color and optional personalization options.
- Confirm phone number, address, policies, shipping and tax settings.
- Test checkout, contact forms, quote forms and artwork intake.
- Fill tracking IDs in theme settings only after accounts are ready.
- Create the Family Reunion Shirt Sale page with handle `family-reunion-shirts-sale` before promoting the summer sale.
