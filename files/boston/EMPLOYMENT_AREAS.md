# Boston: Employment Core Boundaries and Industry Composition

## Research objective
Identify and interpret a high-density employment area with mixed economic functions. The aim is not to certify a unique CBD, reproduce a planning district, or weight firms by brand recognition or market capitalization.

Primary jobs (JT01) represent the highest-earning job per worker in the LODES reference period. In this project, all-industry totals remain totals of primary jobs; secondary positions are excluded. See the [Census LODES methodology](https://www2.census.gov/library/working-papers/2025/adrm/ces/CES-WP-25-52.pdf).

## Scale comparison
Hold grid cells at 250 m and compare Gaussian smoothing bandwidths (kernel standard deviations) of 250, 500, and 1,000 m. Apply a 0.95 quantile rule and track the connected component containing the Phase 1 reference peak, subject to a minimum of 10,000 unsmoothed jobs. Tracking this fixed anchor differs from choosing the largest area independently at each scale.

| Bandwidth (m) | Full-cell area (km²) | Unsmoothed primary jobs | Density cutoff (jobs/km²) |
|---:|---:|---:|---:|
| 250 | 28.375 | 653,618 | 4,410.50 |
| 500 | 48.750 | 732,302 | 3,564.53 |
| 1,000 | 61.125 | 740,736 | 3,394.49 |

These results use a finer grid than the Phase 1 default; the areas should not be treated as the same specification.

## Common area and fixed-cutoff checks
The intersection covers 454 cells, or 28.375 km², and contains 653,618 primary jobs assigned by workplace block representative points. In this experiment, it coincides with the 250 m bandwidth candidate. It contains approximately 88.24% of the jobs in the 1,000 m bandwidth candidate. About 2.662 km² (9.38%) overlaps mapped water.

Agreement across these three specifications is not a confidence probability or validation by independent datasets. To separate changes in numerical cutoffs from changes in bandwidth, the three cutoffs were crossed with all three bandwidths. These nine comparisons show that percentile-induced changes in the cutoff alone do not explain area expansion. Boundaries still depend on the chosen specification.

The union contains 1,012 cells and 754,059 primary jobs. Mutually exclusive agreement classes contain:

| Number of specifications identifying a cell | Cells | Jobs |
|---:|---:|---:|
| 3 | 454 | 653,618 |
| 2 | 292 | 65,361 |
| 1 | 266 | 35,080 |

## Industry composition
The common area includes professional, scientific, and technical services (22.61% of jobs), health care and social assistance (17.23%), educational services (12.12%), and finance and insurance (10.43%). This supports interpreting it as a mixed employment cluster rather than a purely financial or commercial district.

The industry map aggregates unsmoothed CNS01–CNS20 job counts to the same 250 m grid. Selecting an industry changes the displayed measure, not the boundary. Local industry share is industry jobs divided by all jobs in that cell. A minimum total-job threshold mutes small denominators on the share map but does not remove them from summaries.

Count colors rescale with the selected industry and area; share colors remain fixed at 0–100%. Darker cells indicate larger values within the displayed scale, not more institutions, students, or campus acreage. Jobs are assigned using block representative points, not individual buildings.

## PLAN: Downtown as external context
The retrieved PLAN: Downtown polygon covers approximately 0.966 km² and is covered by the common area to numerical precision. It occupies only about 3.41% of the common area. This is not a boundary-accuracy score: a planning district and an employment cluster answer different questions.

Within the common area, the planning polygon contains 125,710 jobs, versus 527,908 outside it. Finance and insurance account for about 20.20% inside and 8.10% outside; educational services account for 3.81% inside and 14.10% outside. These are point-assigned LODES job totals, not a firm census or area-weighted allocation of blocks.

## Limitations and stopping point
Full-cell areas include water. Removing water alone does not establish the correct economic boundary, and smoothing does not model bridges, tunnels, or commuting networks. Industry evidence uses the same LODES source as identification; it is descriptive context rather than independent validation. Planning boundaries are contextual references, not calibration targets. Employer examples do not establish the identity of employers in LODES records.

This stage concludes with a reproducible employment-area definition, sensitivity checks, and a functional interpretation. Transportation accessibility, cross-year stability, and cross-city comparisons remain separate extensions.

## Sources and reproducibility
- [Census LODES](https://lehd.ces.census.gov/data/)
- [Census TIGER water polygons](https://www2.census.gov/geo/tiger/TIGER2024/AREAWATER/)
- [Boston PLAN: Downtown](https://www.bostonplans.org/planning-zoning/planning-initiatives/plan-downtown)

This English brief summarizes the archived Phase 2 outputs. Geometry checks, raw-job reconciliation, industry totals, and fixed-cutoff comparisons were completed during stage closeout. The archived analytical snapshots remain unchanged.
