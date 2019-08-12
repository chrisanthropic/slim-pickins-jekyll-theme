---
layout: post
title: Test Sampling Locations and Extractions
tags:  
- extraction 
---

### Sampling 2 locations to use a test sites for testing a [variety of PCR primers](https://github.com/meschedl/Narragansett_Bay_eDNA/blob/master/test_primers.csv) and extracting from those filters

| Sample Name | Location | Google Earth # | Latitude | Longitude |
|---|----|---|---|---|
| IPT 1 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| ITP 2 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| IPT 3 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| IPT 4 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| IPT 5 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| IPT 6 | India Point Park | 1 | 41°49'2.28"N | 71°23'28.10"W |
| GSOT 1 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 2 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 3 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 4 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 5 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 6 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |
| GSOT 7 | GSO Beach | 17 | 41°29'33.39"N | 71°25'12.72"W |

**Filtering**

Samples from GSO were taken and filtered on March 16th
Samples from India Point Park were taken and filtered on March 18th  

Collection and filtering happen on the same day to minimize degradation of DNA  

Filtering roughly followed the [previous protocol](https://github.com/meschedl/Narragansett_Bay_eDNA/blob/master/notebook/Test-Filter-and-Extraction.md), as well as DNA extraction

- Each replicate represents a 1 liter sample stored in a whirl pak
- Before filtering, the benchtop was wiped down with 10% bleach and DI water
- Samples were filtered with the sample funnel because they were from the same location but with separate filters
- Filters were removed from the funneling apparatus with forceps. Forceps were cleaned with 10% bleach then DI water between uses
- Filters were folded multiple times then stuffed in 1.5mL tubes and frozen at -20 degrees

**DNA Extraction**

DNA was extracted from all samples on the same day: March 20th, using the Qiagen DNeasy Kit and modifications from Renshaw et. al
- Before extraction, the benchtop was wipped down with 10% bleach and DI water
- Added to each tube with the frozen filters:
    * 567µl buffer ATL
    * 63µl Proteinase K
- Samples were digested at 65 degrees C for 6 hours on the Thermomixer and shaking at 600rpm
- After incubation, the filters were taken out of the 1.5mL tubes to get at the liquid with cleaned forceps (same as above). Excess liquid was squeezed out as best as possible with the forceps into new 5mL tubes
- The 1.5mL tubes from the incubation were centrifuged on the tabletop myfuge for 30 seconds to pellet out any dirt or debris
- The supernatant was transferred to the corresponding 5mL tube
- Added to each 5mL tube and then vortexed
    * 630µl buffer AL
    * 630µl 100% EtOH
- The sample had to run through the spin column 3 times.
    * Added 600µl sample to the spin column then centrigued at 8000rpm for 1 minute
    * Transfer column to new collection tube
    * **Repeat above steps twice more to run all sample though the column**
- Added 500µl buffer AW1 to the columns then centrifuged at 8000rpm for 1 minute
- Transferred columns to new collection tubes, added 500µl buffer AW2 and centrifuged at 14000rpm for 3 minutes
- Transferred columns to final 1.5mL tubes
    * Added 50µl warmed (56 degrees C) buffer AE directly to the filter
    * Incubated at room temperature for 5 minutes
    * Centrifuged at 8000rpm for 1 minute
    * **in the same 1.5mL tube** repeated above steps with 30µl warmed buffer AE
- 30µl of extracted DNA was aliquoted into a second working tube to be used for testing and the remaining 50µl will stay as a stock
- DNA is stored in the -20 in a separate box

**Qubit**

- Following this [protocol](https://meschedl.github.io/MESPutnam_Open_Lab_Notebook/Qubit-Protocol/) using the High Sensitivity DNA Kit
- All samples were read twice

| Sample # | Standard 1 (RFU) | Standard 2 (RFU) | DNA Quant 1 (ng/µl) | DNA Quant 2 (ng/µl) |
|------|-----|-----|-------|-------|
| IPT 1 (30) | 51.21 | 24107.3 | 36.8 | 37.0 |
| ITP 2 (30) | 51.21 | 24107.3 | 43.0 | 43.0 |
| IPT 3 (30) | 51.21 | 24107.3 | 47.0 | 47.2 |
| IPT 4 (30) | 51.21 | 24107.3 | 47.0 | 46.8 |
| IPT 5 (30) | 51.21 | 24107.3 | 45.4 | 44.8 |
| IPT 6 (30) | 51.21 | 24107.3 | 19.1 | 19.1 |
| GSOT 1 (30) | 51.21 | 24107.3 | 38.0 | 38.2 |
| GSOT 2 (30) | 51.21 | 24107.3 | 20.6 | 20.6 |
| GSOT 3 (30) | 51.21 | 24107.3 | 41.0 | 41.0 |
| GSOT 4 (30) | 51.21 | 24107.3 | 35.0 | 34.8 |
| GSOT 5 (30) | 51.21 | 24107.3 | 29.2 | 29.2 |
| GSOT 6 (30) | 51.21 | 24107.3 | 30.2 | 30.2 |
| GSOT 7 (30) | 51.21 | 24107.3 | 31.8 | 31.8 |
