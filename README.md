# Sphagnum Shade vs. Warming

Comparing the isolated effects of canopy shading and long-term whole-ecosystem warming on *Sphagnum* moss tissue water content using two independently published datasets from the SPRUCE experiment at Marcell Experimental Forest, Minnesota.

> Primary Dataset: https://mnspruce.ornl.gov/datasets/spruce-sphagnum-growth-and-photosynthesis-responses-to-shading-treatments-2021

> Additional Dataset: https://mnspruce.ornl.gov/datasets/spruce-sphagnum-phytobiome-responses-to-whole-ecosystem-warming-and-elevated-atmospheric 

---

## Research question
> Does increasing shade raise *Sphagnum* water content by as much as long-term warming lowers it — and what does this reveal about whether light or temperature is the more important driver of peatland carbon storage?

---

## Why it matters
- Northern peatlands store ~⅓ of global terrestrial soil carbon — more per unit area than any other ecosystem
- When *Sphagnum* dries out, decomposition accelerates and centuries of stored carbon are released
- Shrub encroachment creates canopy shade — but whether that shade buffers or worsens desiccation was unknown
- This analysis makes a direct controlled comparison not previously done with these newly published datasets

---

## Results

| Hypothesis | Finding | Result |
|---|---|---|
| H1: Shade increases water content | slope = 0.000206/% shade, p = 0.189 | ⚠️ weak support |
| H2: Warming decreases water content | slope = −0.0268/°C, p < 0.0001, R² = 0.281 | ✅ supported |
| H3: Warming stronger driver than shading | 0.241 vs. 0.019 proportion units across full range | ✅ supported |
| H4: CO₂ smaller effect than warming | no significant independent CO₂ effect | ✅ supported |

---

## Pipeline
`raw CSVs` → `QAQC` → `unit conversion` → `linear regression` → `slope comparison` → `visualization`

## Stack
`R` `R Markdown` `tidyverse` `ggplot2` `ggthemes` `kableExtra` `patchwork`

---

