# SheGuidesMe – Performance Testing

This repository contains performance testing work for [sheguidesme.com](https://sheguidesme.com), carried out using Apache JMeter as part of my QA training. It covers key API endpoints (Login, Read Post, Create Post), each tested under increasing concurrent load to evaluate response time, throughput, and stability.

## Objective
To evaluate API performance under increasing load and identify the point at which response time or reliability degrades.

## Tool Used
- Apache JMeter

## Test Approach
For each endpoint, load was increased in stages (10 → 50 → 100 → 150 concurrent users), measuring average response time, percentiles (90/95/99), throughput, and error rate at each stage.

## Endpoints Tested
1. **Login API** (POST) — see `reports/sheguidesme_login_performance_testing.pdf`
2. **Read Post API** (GET) — see `reports/[filename].pdf` *(add once done)*
3. **Create Post API** (POST) — see `reports/[filename].pdf` *(add once done)*

## Summary of Findings
- The Login API showed a sharp increase in response time as load increased, with errors (25.33%) appearing at 150 concurrent users, suggesting a bottleneck in authentication processing.
- *(Add a line here once Read Post / Create Post results are in, comparing them)*

## Files in this Repository
- `jmx/` — JMeter test plans (.jmx) for each endpoint
- `reports/` — Full detailed test reports (PDF) with data for all test stages
- `README.md` — This overview

## Conclusion
Full observations, metrics, and analysis for each endpoint are available in the corresponding PDF report under `reports/`. This README summarizes the project scope and key takeaways only.
