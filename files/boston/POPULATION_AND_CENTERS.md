# Boston: Population Density and Employment Centers

## Research question
Does the choice of reference center materially change the estimated population density gradient in the Boston area?

## Data and study area
Population comes from the ACS 2020–2024 five-year estimates (B01003_001E), with the published margin of error retained. Density is population divided by land area (ALAND) from 2024 TIGER/Line tract boundaries, reported in persons per square mile. The baseline includes 742 tracts whose geometric centroids lie within 20 miles of Boston City Hall. This is neither the municipal boundary nor the metropolitan statistical area. Eleven tracts have zero population estimates; 731 tracts enter the positive-density log regressions.

Employment centers are identified using 2023 LODES workplace primary jobs (JT01, C000). Massachusetts workplace block representative points within 25 miles of City Hall provide the employment search area and smoothing buffer. Distances and areas use the Massachusetts Mainland projection, EPSG:26986, in meters; gradient distances are converted to miles.

Primary jobs (JT01) represent the highest-earning job per worker in the LODES reference period. In this project, all-industry totals remain totals of primary jobs; secondary positions are excluded. See the [Census LODES methodology](https://www2.census.gov/library/working-papers/2025/adrm/ces/CES-WP-25-52.pdf).

## Three reference centers
- **City Hall:** a fixed administrative benchmark.
- **Employment-weighted centroid:** the mean projected location of block representative points, weighted by unsmoothed jobs within the leading candidate area.
- **Strongest employment peak:** the highest retained local maximum of the smoothed surface within that leading area.

The default identification uses 500 m cells, a 1,000 m Gaussian bandwidth (kernel standard deviation), and the 95th percentile of smoothed values evaluated over cells with observed jobs. The threshold is applied to the full grid. Candidate areas connect along shared edges and must contain at least 10,000 unsmoothed jobs; the leading area has the largest job total. Local maxima are compared with eight neighbors, plateaus are collapsed, and a minimum separation filters nearby peaks.

The strongest peak is the principal analytical reference. It is not selected by maximizing the population regression fit. Industry composition and PLAN: Downtown provide substantive context, not proof of a unique CBD center.

## Population gradient
The descriptive model is ln(density) = intercept + slope × distance in miles. Each tract receives equal weight. The implied percentage change per additional mile is 100 × [exp(slope) − 1]. The exponentiated fitted line is not an arithmetic mean prediction of density.

| Reference center | Slope per mile | R² | Fitted decline per mile |
|---|---:|---:|---:|
| City Hall | −0.157792 | 0.441837 | 14.60% |
| Employment-weighted centroid | −0.154638 | 0.433756 | 14.33% |
| Strongest employment peak | −0.157391 | 0.440865 | 14.56% |

These baseline estimates are close. Changing the study radius has a larger effect: the City Hall decline is approximately 19.37%, 18.07%, and 14.60% for the 10-, 15-, and 20-mile samples. This is a comparison across samples, not evidence of a causal distance effect.

Distance-band summaries use total population divided by total land area for tracts grouped by centroid distance. Tracts are not clipped to exact annuli. Zero-population tracts with positive land area remain in those summaries.

## Sensitivity and interpretation
Nine grid–bandwidth specifications and three quantile thresholds were examined. Stability of a reference point does not establish a stable boundary. At the default specification, the leading candidate spans 93.5 km², including approximately 11.71% water. Removing water does not re-estimate the employment surface. Grid connecting paths do not represent roads or commuting routes.

The default peak lies within the retrieved PLAN: Downtown polygon; this is contextual support, not a tuning objective or an official designation of the peak as the CBD center.

## Limitations
The analysis uses straight-line distances and tract geometric centroids. It does not propagate ACS sampling uncertainty, adjust inference for spatial dependence, or estimate causal effects. LODES has coverage and disclosure-protection limitations. Primary jobs are not resident population or building-level workplace observations. ACS and LODES refer to different periods. Planning boundaries serve different purposes from statistical employment areas.

## Sources and reproducibility
- [Census ACS](https://www.census.gov/programs-surveys/acs)
- [Census LODES](https://lehd.ces.census.gov/data/)
- [Census TIGER/Line](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)
- [Boston PLAN: Downtown](https://www.bostonplans.org/planning-zoning/planning-initiatives/plan-downtown)

This English brief summarizes the archived Phase 1 results. The interactive pages may display alternative parameter settings. Archived analytical snapshots remain unchanged.
