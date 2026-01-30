# Life-history trait patterns across tropical vertebrates

This repository contains data processing and analysis workflows used to study
broad-scale patterns of life-history traits across tropical vertebrates,
focusing on amphibians, reptiles (Squamata), and birds.

The project explores how key life-history traits — particularly longevity and
annual fecundity — vary across taxa and environmental gradients, and whether
trade-offs between these traits help explain observed macroecological and
evolutionary patterns in tropical systems.

---

## Background

Life-history theory predicts that organisms face trade-offs in the allocation of
resources to survival, growth, and reproduction. One of the most widely discussed
trade-offs is between longevity and fecundity, where increased investment in
current reproduction may come at the cost of reduced survival.

Despite extensive theoretical development, empirical support for these patterns
remains inconsistent, especially across broad taxonomic groups and in tropical
regions. This project aims to provide a comparative perspective by integrating
trait data with environmental and spatial information across multiple vertebrate
lineages.

---

## General workflow

The analyses implemented in this repository follow three main steps:

1. **Species occurrence curation**  
   Occurrence records are downloaded from GBIF and subjected to a rigorous
   cleaning process, including taxonomic name resolution, spatial filtering,
   coordinate validation, and spatial thinning. This step ensures that species
   distributions used in downstream analyses are reliable and comparable.

2. **Trait and environmental data integration**  
   Cleaned occurrence data are combined with life-history traits (longevity and
   fecundity) and environmental variables to characterize patterns across taxa
   and gradients.

3. **Statistical analyses**  
   Comparative and statistical analyses are used to evaluate relationships
   between life-history traits, test for evidence of trade-offs, and assess how
   these traits respond to environmental variation.

---

## GBIF data processing

The repository includes scripts for automated retrieval and cleaning of GBIF
occurrence data. These scripts:

- Resolve taxonomic names and synonyms using the GBIF backbone
- Filter records based on data quality criteria
- Remove problematic coordinates using CoordinateCleaner
- Apply spatial thinning to reduce sampling bias
- Output cleaned occurrence datasets and summary tables per species

These procedures are intended to support trait-based and comparative analyses,
rather than to describe species distributions per se.

---

## Repository structure

- `data/` – Input data and cleaned datasets  
- `scripts/` – R scripts for data curation and analysis  
- `outputs/` – Processed data products and summaries  

---
