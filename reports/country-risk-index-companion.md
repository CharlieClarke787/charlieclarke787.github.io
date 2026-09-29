# Composite Country Risk Index

**Supporting evidence for Artemis Forecasting | Snapshot target year: 2024**

This is a screening companion to the composite country-risk work in Artemis Forecasting. It follows an ICRG/PRS-style structure but does not use licensed ICRG or PRS data.

## Read this before the number

The 2024 snapshot contains four countries: Russia, Iran, Venezuela, and Syria. IMF and World Bank Worldwide Governance Indicators (WGI) components could not be obtained for this run and are marked missing. No missing value is imputed. The available component is the Freedom House aggregate score, reversed into risk. Since missing component weights are renormalised, each composite equals that one available component.

## Snapshot outputs

| Country | Composite score | Risk band | Available component | Missing components |
| --- | ---: | --- | --- | --- |
| Russia | 88.00 | Very high | Freedom House: 88.00 | WGI governance; IMF macroeconomics |
| Iran | 89.00 | Very high | Freedom House: 89.00 | WGI governance; IMF macroeconomics |
| Venezuela | 87.00 | Very high | Freedom House: 87.00 | WGI governance; IMF macroeconomics |
| Syria | 95.00 | Very high | Freedom House: 95.00 | WGI governance; IMF macroeconomics |

The scale runs from 0 (lower observed institutional/macroeconomic risk) to 100 (higher risk). “Very high” is a screening band, not a forecast.

## Method

When all component groups are present, governance has a 50% weight, macroeconomics 25%, and civic freedom 25%. If a group is missing, the available weights are renormalised. The intended transformations are:

| Component | Indicators and transformation | Weight |
| --- | --- | ---: |
| Governance | World Bank WGI: government effectiveness, political stability/absence of violence, rule of law, and control of corruption. Each estimate on roughly −2.5 to +2.5 is mapped to 100 (highest risk) through 0 (lowest risk). | 50% |
| Macroeconomics | IMF DataMapper: real GDP growth is mapped from +10% = 0 risk to −10% = 100 risk; general government gross debt is mapped from 0% = 0 risk to 150% = 100 risk. Endpoints are clamped. | 25% |
| Civic freedom | Freedom House aggregate total (0–100 freedom) is reversed to risk: `100 − total`. | 25% |

The method uses the latest available observation at or before 2024 for each source. Source years may differ. The results list missing indicators and reject a row with no usable component.

## Use and limitations

Use this number to test a qualitative judgment: does the direction look plausible, which component drives a disagreement, and what evidence should be collected next? It can make assumptions explicit and provide a repeatable baseline for a later snapshot.

It cannot replace country analysis. The index does not model conflict exposure, sanctions, external financing, commodity concentration, exchange-rate stress, institutional nuance, or event timing. The fixed weights and mappings are policy choices, not calibrated probabilities. WGI and Freedom House are perception and expert-coded measures with their own coverage and revision practices. A band should inform questions, not determine a judgment.

## Provenance and limitations

The data files, source list and code used to produce them are in the [Artemis Forecasting repository](https://github.com/CharlieClarke787/artemis-forecasting). The source list records that some IMF requests were refused and that no observations were available for the WGI snapshot. A rerun may change historical values if providers revise their data.

Independent analytical work prepared for portfolio purposes. Not for investment or policy use.
