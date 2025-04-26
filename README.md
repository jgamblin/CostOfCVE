# Cost of CVE Record

This repository contains Jupyter Notebooks that calculates the cost of managing and maintaining the CVE (Common Vulnerabilities and Exposures) Program based on the latest MITRE and NIST contracts. The analysis is based on publicly available data from the [USAspending.gov](https://www.usaspending.gov) and [HigherGov](https://www.highergov.com/) websites.

## Overview

The contract period analyzed in this project spans from **April 17, 2024**, to **April 16, 2025**. During this period, MITRE received **$28,967,283.11** from CISA (Cybersecurity and Infrastructure Security Agency) to manage the CVE Program and Analygence contract with the NVD was worth **$25,000,000**.

[MITRE Contract Link](https://www.usaspending.gov/award/CONT_AWD_70RCSJ23FR0000015_7001_70RSAT20D00000001_7001)
[Analygence Contract Link](https://www.highergov.com/idv/1333ND24DNB770002/)


### Key Findings

- **Cost Per CVE Published During the Contract Period**:  
  - MITRE received **$664.01** for each of the **43,625** CVEs published during the contract period.

  - Analygence contract value was **$573.07** for each of the **43,625** CVEs published during the contract period.

  - The combined cost was **$1,237.07** for each of the **43,625** CVEs published during the contract period.

- **Overall Cost Per CVE in the Database**:  
  - MITRE received **$99.60** for each of the **290,834** CVEs in the CVE database during the contract period.

  - Analygence contract value was **$87.19** for each of the **290,834** CVEs in the CVE database during the contract period.

  - The combined cost was **$188.22** for each of the **286,729** CVEs in the CVE database during the contract period.

## Data Source

## Data Source

The data used in this analysis is sourced from the [CVE List V5 GitHub repository](https://github.com/CVEProject/cvelistV5). This repository contains JSON files with CVE records, organized by year. These files are processed to extract relevant metadata, including publication dates, CVSS scores, and affected products.

The [MITRE Contract](https://www.usaspending.gov/award/CONT_AWD_70RCSJ23FR0000015_7001_70RSAT20D00000001_7001/) was sourced from USASpending.gov.


The [Analygence Contract](https://analygence.com/news/analygence-awarded-position-on-125m-nist-cybersecurity-and-privacy-support-services-capss-blanket-purchase-agreement-idiq/) was source from their website and from [Highergov.com](https://www.highergov.com/idv/1333ND24DNB770002/)