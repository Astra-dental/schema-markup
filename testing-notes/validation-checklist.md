# Schema Markup Validation & Implementation Notes

Notes for validating and deploying the structured data files in this repository for Astra Dental Centre.

## How to implement

1. Copy the JSON object from the relevant file (e.g. `dentist/dentist-localbusiness.json`).
2. Wrap it in a script tag in the page `<head>` or before `</body>`:
   `<script type="application/ld+json"> ... </script>`
3. Use ONE primary business schema (Dentist) sitewide, referenced by `@id`.
4. Add page-specific schema (FAQPage, BreadcrumbList, Service) only on pages where that content is actually visible.

## Validation tools

- Google Rich Results Test: https://search.google.com/test/rich-results
- Schema.org Validator: https://validator.schema.org/
- After deploying, monitor Google Search Console > Enhancements for errors.

## Pre-publish checklist

- [ ] All JSON parses without errors (no trailing commas, balanced braces).
- [ ] `aggregateRating.reviewCount` reflects the REAL number of Google reviews, not the placeholder "100".
- [ ] Individual `Review` items use REAL reviewer names and review text (replace the REPLACE_WITH_... placeholders).
- [ ] FAQPage questions/answers match the visible FAQ content on the page (required by Google).
- [ ] BreadcrumbList positions and URLs match the actual page hierarchy.
- [ ] Logo and image URLs resolve to real, publicly accessible files.
- [ ] Address, phone, hours, and social links match the live site.
- [ ] Confirm postal code and geo coordinates are accurate (verify against Google Business Profile).

## Important compliance notes

- Do NOT inflate ratings or review counts. Inflated or fabricated review data violates
  Google's structured data guidelines and can lead to manual penalties.
- Only mark up content that is genuinely present and visible to users on the page.
- Keep NAP (Name, Address, Phone) consistent across schema, the website, and Google Business Profile.

## Source of truth

Live site: https://astradentalcentre.com/
Business: Astra Dental Centre, Unit 120, 20061 Fraser Hwy, Langley, BC
Phone: 604-533-8806 | Email: reception@astradentalcentre.com
