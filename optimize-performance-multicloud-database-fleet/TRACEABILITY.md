# Source Traceability

Estimated Time: 90 minutes

## Source Classification

| Workshop area | Source | Owner / source class | Evidence type | Used as | Notes |
| --- | --- | --- | --- | --- | --- |
| Complete tutorial content | Supplied `LiveLab.html` export from the user's Downloads folder | Oracle-owned/internal | prose, headings, task steps, links | format-translated to Markdown | Visible wording, section order, and task order were preserved; the learner-facing Reference material section was removed at the user's request. |
| Complete tutorial visuals | Supplied `LiveLab_files/` attachment bundle | Oracle-owned/internal | screenshots and diagrams | copied locally and referenced from `images/` | Image filenames were lowercased and normalized only to satisfy LiveLabs path rules. |
| Optional-task screenshots | Local `em-omc` checkout, branch `feature/optimize-performance-multicloud-database-fleet` | Oracle-owned/internal | screenshots for Exadata capacity, SQL Explorer, ADDM Spotlight, Exadata Cost Management, and dashboards | copied locally with a `branch-` filename prefix and added under Task 9 | The existing source screenshots were retained; branch screenshots were added for the optional modules. |
| Reference material | URLs already present in the supplied HTML | Oracle-owned/internal | linked documentation, blog, and Oracle LiveLabs source | recorded as source provenance | The learner-facing Reference material section was removed at the user's request. |

## Embedded Asset Provenance

- Shared Get Started and Need Help pages are linked from Oracle's LiveLabs common CDN, following the existing Database Management Demo Mode workshops. Desktop and tenancy use the cloud-login and Free Tier help pages; sandbox uses the LiveLabs login and help pages.
- These Oracle-owned shared pages and their embedded assets are referenced remotely without copying or modifying them. Existing lab text and screenshots are unchanged.

- The source HTML references Oracle Confluence attachments and Oracle-owned `oracle-livelabs` GitHub images.
- The local output contains 43 image files copied from the supplied attachment folder. No new images were generated and no visual content was edited.
- The local output now contains 41 additional branch screenshots for the five optional modules in Task 9. No screenshot pixels were edited.
- CSS files from the Confluence export were not copied because they are not referenced by the LiveLabs Markdown renderer.

## Approval and Attribution

- External/non-Oracle sources: none identified.
- Unclear sources: none identified from the supplied export and attachment names.
- Current-build source-owner approval: not required under the source classification above.
- Learner-facing public-source attribution: no new attribution was added; the source links remain recorded in this traceability file after removing the learner-facing Reference material section.

## Transformation Notes

- The source was found as `LiveLab.html` (singular) with the matching `LiveLab_files` folder; this is the supplied artifact corresponding to the requested `LiveLabs.html`.
- The HTML body was converted to Markdown without editorial rewriting.
- Image references were converted to local Markdown image references with meaningful alt text where the source omitted alt text.
- Optional-task screenshots from the requested branch were inserted as image references only; existing task wording and sections were not rewritten.
- The Introduction and all four labs include the exact author and contributor acknowledgements supplied by the workshop author. Each lab also includes the approved Introduction, Objectives, and Prerequisites sections. Estimated workshop time remains on the Introduction page.

## Acknowledgements

<!-- Traceability metadata for the supplied LiveLabs source package. -->
