# Traceability Summary

Estimated Time: 5 minutes

## Source Classification

- Oracle-owned/internal sources: the Oracle Confluence view-source export supplied as `LiveLab.html`; its internal Confluence attachments and screenshots.
- Oracle-owned/public sources: the Oracle LiveLabs `em-omc` GitHub content referenced by the HTML; the Oracle Database ADDM Spotlight blog.
- External/non-Oracle sources: none identified.
- Unclear or mixed-ownership sources: none currently identified after review. Embedded assets remain subject to final publication clearance by the workshop SME.
- Current-build source-owner approval confirmed for external or unclear sources and embedded assets: yes. The workshop author confirmed approval in the current build request on 2026-09-14.
- Attribution or rights review needed: no additional third-party attribution was identified. Confirm that internal Confluence screenshots are approved for the intended LiveLabs audience before publication.

## Embedded Asset Review

| Asset | Parent Source | Asset Type | Owner / Source Class | Used As | Approval / Attribution / Rights Notes |
| --- | --- | --- | --- | --- | --- |
| `fleet-health/images/*` | Oracle Confluence export and local attachments | screenshot | Oracle-owned/internal | reused as local workshop screenshots | Current-build approval confirmed; final audience clearance remains an SME check |
| `performance-analysis/images/*` | Oracle Confluence export and Oracle LiveLabs GitHub images | screenshot | Oracle-owned/internal and Oracle-owned/public | reused as local workshop screenshots | Current-build approval confirmed; no remote image hotlinks retained |
| `capacity-planning/images/*` | Oracle LiveLabs GitHub images referenced by the source export | screenshot | Oracle-owned/public | reused as local workshop screenshots | Current-build approval confirmed; no remote image hotlinks retained |

## Source Traceability

| Workshop Area | Source | Owner / Source Class | Evidence Type | Used As | Approval / Attribution / Rights Notes |
| --- | --- | --- | --- | --- | --- |
| Introduction | `LiveLab.html`, supplied Oracle Confluence view-source export | Oracle-owned/internal | claims, environment assumptions, outcomes | summarized and reorganized | Internal provenance only; not exposed in learner-facing acknowledgements |
| Lab 1 | `LiveLab.html`, Demo Mode and Fleet Summary sections | Oracle-owned/internal | navigation, commands, screenshots | adapted into guided steps | Local screenshots copied into `fleet-health/images/` |
| Lab 2 | `LiveLab.html`, DBM performance and SQL Insights sections | Oracle-owned/internal and Oracle-owned/public | navigation, claims, screenshots | adapted and summarized | Public Oracle blog is linked under Learn More; internal sources remain unlisted in learner-facing text |
| Lab 3 | `LiveLab.html`, Capacity Planning and optional modules sections | Oracle-owned/public and Oracle-owned/internal | navigation, feature descriptions, screenshots | adapted and reorganized | The source did not provide a validated SQL Explorer query, so no runnable SQL was invented |

## Attribution Notes

- The external-source gate was satisfied before workshop authoring. The workshop author confirmed current-build approval after being shown that the HTML included internal Confluence content and public GitHub/blog material.
- Add learner-facing `Source` links only for external-facing public URLs.
- Confirmed approval is recorded in each learner-facing acknowledgement as `Built with permission from the author(s).`
- Do not list Oracle-internal, Oracle-owned private, local, SharePoint, iCloud, unpublished, or confidential sources in learner-facing acknowledgements.
- Record non-public provenance here only when auditability is needed.
- The learner-facing files use local copies of the screenshots and do not depend on the saved HTML or remote image paths.

## Open Gaps

- Internal screenshots need final SME/publication clearance for the intended LiveLabs audience.
- The SQL Explorer module still needs a validated workshop query if the course owner wants a runnable example.
- Product navigation labels and Demo Mode data can change; perform a product-owner review before publication.

## Acknowledgements

* **Traceability Compiled By** - Codex
* **Last Updated By/Date** - 2026-09-14
