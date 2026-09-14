# Workshop Details

## Short Description

Use OCI Database Management and Ops Insights Demo Mode to investigate a database performance signal across a multicloud fleet. Review current health, SQL activity, historical findings, capacity trends, and forecasts before recommending a next action.

## Long Description

Operations teams need to move quickly from a fleet-level alert or hotspot to the database, workload, or capacity evidence behind it. This 90-minute workshop uses curated Demo Mode data so learners can practice that workflow without provisioning a database or generating a workload.

Learners begin in Database Management Fleet Summary, select a populated database, and review availability, activity, I/O, memory, storage, Performance Hub, SQL Monitoring, AWR Explorer, and ADDM Spotlight. They then use Ops Insights SQL Insights and Capacity Planning to determine whether the signal is isolated or systemic, current or recurring, and likely to require tuning, monitoring, reclamation, resizing, autoscaling, or further investigation.

## Workshop Outline

1. Introduction
2. Lab 1: Assess Fleet Health and Select a Database
   - Enable Database Management Demo Mode.
   - Review Fleet Summary and select a populated investigation target.
3. Lab 2: Diagnose Database and SQL Performance
   - Compare database health, Performance Hub, and SQL Monitoring evidence.
   - Add historical context with AWR Explorer and ADDM Spotlight.
   - Correlate SQL patterns across the fleet with Ops Insights SQL Insights.
4. Lab 3: Correlate Capacity, Forecasts, and Optional Modules
   - Review database capacity, growth, unused capacity, and forecasts.
   - Explore one optional Exadata, SQL, ADDM, cost, or dashboard module.
   - Reconcile data differences and write an evidence-backed recommendation.

## Workshop Prerequisites

- OCI Console access to a compartment where Database Management and Ops Insights Demo Mode are available.
- Permission to complete any policy workflow shown while enabling Demo Mode.
- A modern web browser.

Estimated Time: 90 minutes

## Acknowledgements

* **Source approval** - The workshop author confirmed approval to use the provided source material for this build. Built with permission from the author(s).
* **Author** - Workshop owner to be assigned
* **Last Updated By/Date** - 2026-09-14

## Notes

- Keep this file aligned with the final manifest and lab titles.
- Keep the long description learner-focused. Do not say the workshop was created from a blog, prompt, or source format.
- The 90-minute estimate includes optional feature exploration. The core path is shorter when the optional module is deferred.
- This workshop does not include FreeSQL. The source does not provide a validated runnable SQL statement for SQL Explorer.
