# Hack for LA: 311 + Transit Proximity MVP

This repository contains exploratory data analysis (EDA) and MVP work investigating the relationship between Los Angeles 311 service requests and their proximity to LA Metro infrastructure (rail and bus stops).

The project supports Hack for LA’s civic data initiatives by building a reproducible pipeline to link 311 requests with public infrastructure, enabling both descriptive and causal analysis of how city services interact with transit hubs.

## Current Focus

- Metro rail stops -> MVP notebook (`metro_311_project_setup.ipynb`)
  - Per-capita 311 request rates by distance bands
  - Visualization of request type distributions near stations
- Metro bus stops -> Control notebook (`metro_311_bus_control.ipynb`)
  - Same analysis replicated for bus stop coverage 
  - Provides a baseline to test whether rail-specific effects exist

## Key Insights So Far

- Most requests cluster within walking distance of transit, especially bus stops
- Raw request counts can be misleading; population normalization is critical
- Certain categories (graffiti, bulky items) appear disproportionately near transit infrastructure

## Next Steps

- Directly compare bus vs. rail results
- Use regression/matching to test whether rail stops have unique effects beyond urban density
- Extend analysis to multiple years (2020–2024)

## Links

- [Hack for LA GitHub Issue](https://github.com/hackforla/data-science/issues/107)

## Structure

- `data/`: Cleaned datasets (no large raw files)
- `notebooks/`: Analysis notebooks
- `scripts/`: Reusable code
- `outputs/`: Summary visuals
- `docs/`: MVP charter, slides
- `.gitignore`
- `README.md`

