# Lab 3: Correlate Capacity, Forecasts, and Optional Modules

## Introduction

Use Ops Insights Capacity Planning to connect the database-level diagnosis with a fleet-level response. Compare allocation, utilization, growth, unused capacity, and forecast demand. Then choose one optional module to explore if the relevant data is populated.

### Objectives

In this lab, you will:

- Review Oracle Database capacity across CPU, storage, memory, and I/O.
- Compare current usage with growth and forecast views.
- Choose a response based on database and fleet evidence.
- Explore one optional Exadata, SQL, ADDM, cost, or dashboard capability.

Estimated Time: 25 minutes, plus optional module time

## Task 1: Forecast Database Capacity

Capacity Planning provides a longer-term view of allocation, utilization, growth, unused capacity, and forecast demand.

1. Open **Ops Insights → Capacity Planning → Oracle Databases**.
    ![Oracle Database Capacity Planning overview](images/capacity-planning.png)
2. Set **Time Range** to **Last 90 days**, when that range is available.
    ![Capacity Planning time-range filter](images/capacity-filter.png)
3. Review database inventory and aggregate allocation and utilization for CPU, storage, memory, and I/O.
    ![Capacity Planning inventory](images/capacity-inventory.png)
4. Review top consumers and growth views for CPU, storage, and memory.
5. Apply database type or tag filters when they help isolate the affected fleet segment.
6. Open **CPU → Insights** and review the 30-day high-utilization forecast.
    ![CPU Insights forecast](images/cpu-insights.png)
7. Select a populated database or group for a focused trend and forecast view.
8. Compare average usage, maximum usage, allocation, utilization, and usage change.
9. Compare the available linear regression, seasonality-aware, and AutoML forecast views. Record the training period and confidence interval when shown.
10. Open **Storage** and check whether unused capacity or the storage forecast changes your recommendation.
    ![Storage Insights forecast](images/storage-insights.png)

Record:

- Resource analyzed: `[CPU/storage/memory/I/O]`
- Forecast horizon or time range: `[range]`
- Top consumer or group: `[consumer]`
- Allocation versus usage: `[observation]`
- Forecast model: `[model or N/A]`
- Forecast risk: `[risk]`
- Recommended response: `[action]`

**Checkpoint:** Connect the database-level evidence from Database Management to the fleet-level decision in Ops Insights.

## Task 2: Explore One Optional Service Module

Choose one populated module for the event version. Complete the remaining modules in a self-paced session. If a module has no data, return to Capacity Planning and select another option.

### Option A: Exadata Capacity Planning

Exadata Insights extends capacity planning to Exadata systems, hosts, VM clusters, databases, and storage servers.

1. Open **Exadata Insights** and review aggregate current and forecast utilization.
    ![Exadata Insights overview](images/exadata-insights.png)
2. Select a populated Exadata system and review **Rack and Key Metrics**.
    ![Exadata systems](images/exadata-systems.png)
    ![Exadata rack and key metrics](images/exadata-rack-metrics.png)
3. Open **Metrics by Database** and compare CPU usage by database and host.
    ![Exadata metrics by database](images/exadata-metrics-by-database.png)
    ![Exadata metrics by database and host](images/exadata-metrics-by-database-host.png)
4. Use **Allocation (CPU)** for size and **Usage Change (%)** for color to identify growing or shrinking consumers.
    ![Exadata allocation and usage change](images/exadata-allocation-usage-change.png)
5. Drill into host and database trend or forecast views.
    ![Exadata host trend](images/exadata-host-trend.png)
6. Select **Usage (average active CPU)** for size and **Utilization (%)** for color, then enable **Show Unused Capacity**.
    ![Exadata unused host capacity](images/exadata-unused-host.png)
7. Repeat the unused-capacity view by VM cluster.
    ![Exadata unused VM cluster capacity](images/exadata-unused-vm-cluster.png)
8. Review **Metrics by Host** and **Exadata Storage Server** for aggregate trends, forecasts, and individual series.
    ![Exadata metrics by host](images/exadata-metrics-by-host.png)
    ![Exadata storage server forecast](images/exadata-storage-server-forecast.png)

**Module output:** Identify one Exadata host, VM cluster, database, or storage resource that is over-utilized, growing, forecasted to constrain demand, or under-used.

### Option B: SQL Explorer

Use SQL Explorer to create a focused fleet visualization. Do not invent a query or a result when the environment does not provide a validated example.

The screenshots below illustrate the UI flow. Use the validated query and current data supplied for the event environment.

1. Open **SQL Insights → SQL Explorer**.
    ![SQL Explorer](images/sql-explorer-main.png)
2. In basic mode, run a validated workshop query supplied by the event instructor or course owner that aggregates CPU time or elapsed time by database and SQL ID.
    ![SQL query](images/sql-query.png)
3. Sort by descending resource use and limit the result set.
    ![SQL query results](images/sql-query-table.png)
4. Display the result as a stacked bar chart.
    ![SQL stacked-bar visualization](images/sql-query-visual.png)
5. Open **Advanced** mode and inspect available views, columns, and sample queries.
    ![SQL Explorer Advanced mode](images/sql-explorer-advanced.png)
    ![SQL Explorer views and queries](images/sql-explorer-view-queries.png)
    ![SQL Explorer available views](images/view-queries.png)
    ![SQL Explorer column details](images/sql-column-details.png)
6. Modify one filter or grouping and rerun the visualization.
    ![Clear SQL query](images/sql-explorer-clear.png)
    ![Updated SQL query](images/sql-query1.png)
    ![Updated SQL query results](images/sql-query-table1.png)
    ![Updated SQL visualization](images/sql-query-visual1.png)

**Module output:** Produce one fleet SQL visualization and explain the query dimensions used.

### Option C: ADDM Spotlight

Use ADDM Spotlight to prioritize recurring or high-impact findings over time.

The screenshots illustrate the workflow; database names and values may differ in Demo Mode.

1. Open **Database Insights → ADDM Spotlight**.
    ![ADDM Spotlight navigation](images/addm-spot01.png)
2. Review the database listing, findings count, maximum overall impact, and most frequent category.
    ![ADDM Spotlight database listing](images/addm-spot02.png)
3. Filter by time range and search for a populated database.
    ![ADDM Spotlight filtered database listing](images/addm-spot03.png)
4. Review the summary timeline, **Findings**, **Recommendations**, and **Database Parameters**.
    ![ADDM Spotlight findings](images/addm-spot04.png)
    ![ADDM Spotlight recommendations](images/addm-reco.png)
    ![ADDM Spotlight database parameters](images/addm-dbpars.png)
5. Compare one impactful finding with the Database Management or Capacity Planning evidence.

**Module output:** Record the highest-impact finding and the recommended next action.

### Option D: Exadata Cost Management

Use cost and usage views to identify a showback, chargeback, or resource-optimization opportunity.

The screenshots illustrate the controls; available groupings and values may differ in the current environment.

1. Open **Exadata Insights → Exadata Cost Management**.
    ![Exadata Cost Management](images/opsi-chargeback-main.png)
2. Select a populated Exadata system.
    ![Exadata Cost Management details](images/opsi-chargeback-details.png)
3. Review actual cost, attributed cost, VM cluster CPU utilization, and the database table.
4. Set **Primary grouping** to **CostCenter** and **Secondary grouping** to **Environment**, when available.
    ![Primary cost grouping](images/primary-grouping.png)
    ![Cost grouping selector](images/opsi-chargeback-grouping.png)
    ![Secondary cost grouping](images/opsi-chargeback-grouping2.png)
5. Select a chart segment to filter the database table to one cost center or environment.
    ![Cost-center selection](images/cost-center-01.png)
6. Review usage and charge trends, then switch to table data.
    ![Usage and charge trends](images/trend-charts.png)
    ![VM cluster trend selection](images/deselect-test-vmc1.png)
    ![Show table data](images/select-show-table.png)
    ![Cost table data](images/table.png)
7. Inspect how OCI standard or free-form tags support cost-center or line-of-business filtering.

**Module output:** Identify a cost center or environment with a resource-usage or chargeback optimization opportunity.

### Option E: Ops Insights or Database Management Dashboards

Use a saved dashboard to shorten the path from a fleet signal to database and SQL analysis.

The screenshots illustrate the dashboard flow; dashboard names and insights may vary by environment.

1. Open **Dashboards** and review the out-of-the-box dashboard list.
    ![Ops Insights dashboards](images/opsi-dash-main.png)
    ![Dashboard navigation](images/opsi-left-dash.png)
2. Open **(Demo) SQL Insights – Fleet Analysis**, when available.
    ![SQL Insights Fleet Analysis dashboard](images/opsi-demo-insights-fleet-analysis.png)
3. Select the **Degrading SQL** insight to list affected databases.
    ![Degrading SQL insight](images/opsi-degrading-sql.png)
    ![Databases with degraded SQL](images/opsi-db-with-degraded-sql.png)
4. Open a database analysis view.
    ![Database analysis](images/opsi-db-analysis.png)
5. Select **Degraded plan changes**, when available.
    ![Degraded plan changes](images/opsi-degraded-plan.png)
6. Open a SQL analysis view for one SQL ID.
    ![SQL ID analysis](images/opsi-sql-id-analysis.png)

**Module output:** Explain how a saved dashboard shortens the path from a fleet signal to SQL investigation.

## Task 3: Reconcile Data Differences and Make a Recommendation

Demo Mode data is curated and can change. Follow the evidence in the current environment rather than waiting for a fixed value or exact count.

1. If **CRMCDB** is absent or empty, select another database with populated charts.
2. If Performance Hub, SQL Monitoring, AWR Explorer, or ADDM Spotlight is unavailable for the selected database, return to Fleet Summary and select another populated target.
3. If the exact DBM SQL ID is absent from SQL Insights, use a high-impact SQL statement with a related degradation, plan-change, CPU, or I/O pattern.
4. If a forecast view is empty, use a populated aggregate CPU or storage view and document the visible trend.
5. If Exadata data is unavailable, complete Database Capacity Planning and treat Exadata modules as optional.
6. Do not fabricate a target, finding, metric, SQL ID, or forecast value.
7. Write a final recommendation that states the evidence, the issue classification, and the next action.

Record:

- Evidence from DBM: `[database-level evidence]`
- Evidence from OPSI: `[fleet-level evidence]`
- Issue classification: `[SQL/workload/resource/availability/insufficient evidence]`
- Recommended response: `[tuning/monitoring/reclamation/resizing/autoscaling/further investigation]`

## Acknowledgements

* **Source approval** - The workshop author confirmed approval to use the provided source material for this build. Built with permission from the author(s).
* **Author** - Workshop owner to be assigned
* **Last Updated By/Date** - 2026-09-14
