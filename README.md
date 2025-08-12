![Static Badge](https://img.shields.io/badge/Activity_Status-Archived-red)

## Overview

Enclosed is the code used for the second PopHIVE prototype dashboard, which transitions the code from an RShiny-based implementation to a JavaScript-based one for better performance. This repository includes the code for generating the JavaScript version of the dashboard, referencing data from the R-based version found in [PopHIVE/DSDE-PopHIVE](https://github.com/PopHIVE/DSDE-PopHIVE). During its development, the RShiny-based prototype was still being updated, so some of these updates are not reflected in this version.

The code was originally copied from a repository in the [YSPH Data Science and Data Equity](https://github.com/ysph-dsde) (YSPH-DSDE) GitHub Organization and was copied into the [PopHIVE](https://github.com/PopHIVE) GitHub Organization Aug 12th, 2025. At the time of transfer, the YSPH-DSDE GitHub Organization codebase was no longer being actively contributed to and had been archived.

The dashboard deployment can be found here: _____.

**Dates active:** Mar 10th – May 9th, 2025

&nbsp;

![GitHub Repo stars](https://img.shields.io/github/stars/PopHIVE/PopHIVE-Prototype) ![GitHub watchers](https://img.shields.io/github/watchers/PopHIVE/PopHIVE-Prototype) ![GitHub forks](https://img.shields.io/github/forks/PopHIVE/PopHIVE-Prototype) [![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc/4.0/)

![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/PopHIVE/PopHIVE-Prototype) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/PopHIVE/PopHIVE-Prototype) ![GitHub Release Date](https://img.shields.io/github/release-date/PopHIVE/PopHIVE-Prototype) ![GitHub repo size](https://img.shields.io/github/repo-size/PopHIVE/PopHIVE-Prototype)

![GitHub contributors](https://img.shields.io/github/contributors/PopHIVE/PopHIVE-Prototype) ![GitHub last commit](https://img.shields.io/github/last-commit/PopHIVE/PopHIVE-Prototype) ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/PopHIVE/PopHIVE-Prototype) ![GitHub language count](https://img.shields.io/github/languages/count/PopHIVE-Prototype) ![GitHub top language](https://img.shields.io/github/languages/top/PopHIVE/PopHIVE-Prototype)


# PopHIVE Prototype Aims and Scope

## Aims

**Primary goal:** Reproduce [PopHIVE/DSDE-PopHIVE](https://github.com/PopHIVE/DSDE-PopHIVE) as it looks since March 10th, 2025 in JavaScript with one additional page as a simple landing page. The original outline was borrowed from a previous project, with the most original version reflected in [PopHIVE/PopHIVE](https://github.com/PopHIVE/PopHIVE). Professor Dan Weinberger shared some preferred color pallets for the plots: [saturated](https://colorbrewer2.org/#type=qualitative&scheme=Paired&n=10) and [muted](https://colorbrewer2.org/#type=qualitative&scheme=Set3&n=10).

**Secondary goal:** Suggest improvements on website structure, organization, and aesthetics. Give advice on best practices that are currently reflected in the DSDE-PopHIVE Quarto file and best practices that need to be implemented going forward. NOTE: we do not have a set branding (website color palette, font families, etc.) for PopHIVE. We are using the YSPH logo and favicon for the time being.

**Tertiary goal:** Add plot blocks into the dashboard webpage skeleton for recently harmonized and cleaned datasets from new domains of research.

## Scope

- Two webpages:

    1. Landing page with the title, authors, and link to the dashboard.
    2. Dashboard that is a reproduction of DSDE-PopHIVE as it is as of March 10th.
 
- Three prepared datasets:

    1. Respiratory_Infections.gz.parquet (source DSDE-PopHIVE/Data - [file URL](https://github.com/PopHIVE/DSDE-PopHIVE/blob/main/Data/Respiratory_Infections.gz.parquet))
    2. Respiratory_Infections_Wastewater.gz.parquet (source DSDE-PopHIVE/Data - [file URL](https://github.com/PopHIVE/DSDE-PopHIVE/blob/main/Data/Respiratory_Infections_Wastewater.gz.parquet))
    3. Opioid_Overdoses.csv (source DSDE-PopHIVE/Data - [file URL](https://github.com/PopHIVE/DSDE-PopHIVE/blob/main/Data/Opioid_Overdoses.csv)) and [subsets converted to parquet](https://github.com/PopHIVE/DSDE-PopHIVE/tree/main/Data/Opioid%20Overdoses)

- Plot types:

    1. Within one data source (i.e. RSV-NET, NSSP, Epic Cosmos, etc.) that show rates and counts stratified by geolocation, age, sex, and race/ethnicity.
    2. Between data sources that show scaled counts. This version might have a lot of NA's.

  NOTE: Reference [PopHIVE/data-gov](https://github.com/PopHIVE/data-gov) file `Suggested Static Plots.R` for guidance on plotting from the three prepared datasets.


## Legal Disclaimer

These data and PopHIVE statistical outputs are provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors, contributors, or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the data or the use or other dealings in the data.

The PopHIVE statistical outputs are research tools intended for use in the fields of public health and medicine. They are not intended for clinical decision making, are not intended to be used in the diagnosis or treatment of patients and may not be useful or appropriate for any clinical purpose. Users of the PopHIVE statistical outputs should be aware of their responsibilities to ensure the ethical and appropriate use of this technology, including adherence to any applicable legal and regulatory requirements.

The content and data provided with the statistical outputs do not replace the expertise of healthcare professionals. Healthcare professionals should use their professional judgment in evaluating the outputs of the PopHIVE statistical outputs.
  
