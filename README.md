# 🦉 Brown-Winged Owl Habitat Conservation Planning

<p align="center">
  <img src="./brown_owl_map.jpg" alt="Brown-Winged Owl Map" width="600"/>
</p>

A GIS-based spatial analysis project for forest management and wildlife conservation, focusing on nesting and foraging zones of the **(fictitious) brown-winged owl** in Northern Lower Michigan. The project supports timber planning by modeling areas restricted due to sensitive wildlife presence.

---

## Project Overview

The objective of this lab was to analyze spatial patterns in owl habitat use to support conservation-oriented forest management. Key goals included:

- Identifying **vegetation types used for nesting**
- Determining **proximity to foraging habitats**
- Calculating **area loss for timber harvest** due to nest buffers
- Producing spatial visualizations and tabulated summaries

---

## Technologies and Tools Used

- **ArcGIS Desktop**  
  - Spatial Join  
  - Attribute Queries  
  - Symbology Tools  
  - Buffer, Clip, Near, and Project Tools  
  - Geometry and Field Calculations  
- **Coordinate Systems:**
  - Input: WGS 1984 (GPS)
  - Projected Output: Same as `land_cov.shp` using `NAD_1927_To_WGS_1984_3`
- **Data Formats:**
  - `.shp`, `.csv`, `.dbf`
- **Base Files:**
  - `land_cov.shp`, `owl_nests_loc.csv`

---

## Analytical Results

### Nesting Preferences by Vegetation

| Vegetation Type    | Number of Nests | % of Total Nests |
|--------------------|------------------|------------------|
| Oak                | 32               | 68.09%           |
| Aspen              | 11               | 23.40%           |
| Northern Hardwood  | 3                | 6.38%            |
| Upland Mixed       | 1                | 2.13%            |

> Owls show strong preference for oak and aspen, likely due to protection and foraging proximity.

---

### Nest-to-Foraging Site Distances

| Metric   | Distance (meters) |
|----------|-------------------|
| Minimum  | 6.88              |
| Maximum  | 308.68            |
| Average  | 39.76             |

> Nests are typically located close to foraging zones in herbaceous openings ≥ 0.4 ha.

---

### Forest Area Lost Due to Protection Buffers

| Forested Type         | Area Owned (ha) | Lost Area (ha) | % Lost |
|------------------------|-----------------|----------------|--------|
| Oak                    | 3,504.35        | 188.22         | 5.37   |
| Aspen                  | 1,248.08        | 67.54          | 5.41   |
| Northern Hardwood      | 473.41          | 20.07          | 4.24   |
| Upland Mixed           | 123.46          | 7.75           | 6.28   |
| Others (total)         | 329.29          | 2.76           | —      |
| **Total Forested Area**| **5,678.59**    | **286.34**     | **5.04** |

> Oak leads in absolute loss; upland mixed leads in % loss due to smaller base area.

---

## Key Findings

- **Preferred Nesting**: Oak and aspen dominate nest locations.
- **Proximity Advantage**: Owls tend to nest within 40m of their foraging areas.
- **Impact on Logging**: 286.34 ha of forested land becomes restricted, with oak losing the most area.

---

## Notes

- The brown-winged owl is fictitious. This lab was created as an instructional GIS exercise simulating real-world wildlife planning.
- The map includes synthetic nesting data but follows valid analytical methods suitable for use in forestry and environmental contexts.

> **Created by:** Oscar Babin
> **Date:** September 2023
