# How a New Yorker is living rent free because of broken, unchecked renting subsidy

**Apartment 2L**

This is a data journalism thesis piece about a gap in how New York City tracks its own rent-stabilized housing stock. It centers on Samuel O'Hana's lawsuit against his landlord at 157 Huron Street in Greenpoint, Brooklyn — an apartment that was quietly reclassified as exempt from rent stabilization in 2008 on a filing that contradicted itself, and nobody caught it for nine years.

**Live site:** https://amandamiriamfernandez.github.io/Rent_Stabilization/

## What's in here

- `index.html` — the story, with a scrollytelling map, a rent-history timeline chart, and a borough rent-burden breakdown chart
- `nyc_zips.geojson` — NYC ZIP code boundaries used for the map
- `zip_rentstab_vs_burden.csv` — DHCR building registrations joined against Census rent-burden figures, by ZIP code

## The data

DHCR's 2024 rent-stabilization building registrations, joined against Census ACS Table B25070 rent-burden estimates, for every ZIP code in New York City. The apartment-specific rent history comes from DHCR's registration filings for 157 Huron St., Apt. 2L, and from NYC Rent Guidelines Board apartment orders (used to project what the unit would have legally cost had it stayed rent-stabilized after 2007).

## A few things I found

- Bushwick has the highest concentration of rent-stabilized housing of any ZIP code in the city, and its renters are still severely burdened at almost exactly the citywide rate anyway
- The Bronx has the highest share of severely burdened renters despite real stabilized supply (7,504 buildings); Staten Island combines high burden with almost no stabilized housing at all
- DHCR doesn't publish which specific buildings have stabilized units, only aggregated totals by state assembly and senate district — researchers have to reconstruct building-level counts from property tax bills instead
- There's no public tool that lets a tenant check whether their own unit's status still matches its paper trail; Samuel O'Hana had to request his rent registration history from DHCR directly, page by page, going back to 1984

## Built with

- D3.js
- A NYC ZIP code choropleth + bubble map (rent burden and stabilization density)
