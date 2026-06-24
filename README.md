# Astra Dental Schema Markup

Repository for Astra Dental Centre structured data (JSON-LD) files, schema templates, and implementation notes.

Website: https://astradentalcentre.com/

## Purpose

This repository organizes and backs up the schema markup used across the Astra Dental Centre website. Each folder holds a JSON-LD file ready to be embedded in a `<script type="application/ld+json">` tag.

## Repository structure

| Folder | File | Schema type |
| --- | --- | --- |
| `dentist/` | `dentist-localbusiness.json` | Dentist / LocalBusiness (primary business entity) |
| `faq/` | `homepage-faq.json` | FAQPage |
| `review/` | `aggregate-rating.json` | AggregateRating + Review |
| `service/` | `dental-services.json` | Service + OfferCatalog |
| `breadcrumb/` | `service-page-breadcrumb.json` | BreadcrumbList |
| `organization/` | `organization.json` | Organization |
| `testing-notes/` | `validation-checklist.md` | Validation & implementation guide |

## Business reference (source of truth)

- **Name:** Astra Dental Centre
- **Address:** Unit 120, 20061 Fraser Hwy, Langley, BC
- **Phone:** 604-533-8806
- **Email:** reception@astradentalcentre.com
- **Dentist:** Dr. B. Kumar Potluri (practising since 1996; Invisalign & CEREC certified)
- **Hours:** Mon & Fri 10:00-19:00; Tue-Thu & Sat 09:00-17:00; Sun closed
- **Rating:** 4.9 stars on Google

## How to use

1. Open the JSON file for the schema type you need.
2. Copy the JSON object and wrap it in a script tag in the page head.
3. Validate with the Google Rich Results Test before publishing.
4. See `testing-notes/validation-checklist.md` for the full pre-publish checklist.

## Important notes

- `reviewCount` values and individual `Review` items are PLACEHOLDERS. Replace them with real Google review data before publishing - do not inflate or fabricate ratings.
- FAQ schema must match the FAQ content that is actually visible on the page.
- Keep Name / Address / Phone consistent across schema, website, and Google Business Profile.
- Do not commit any API keys, tokens, or tracking IDs to this repository.
