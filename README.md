# Cost of CVE Record

This repository contains a Jupyter Notebook that calculates the cost of managing and maintaining the CVE (Common Vulnerabilities and Exposures) Program based on the latest MITRE contract. The analysis is based on publicly available data from the [USAspending.gov](https://www.usaspending.gov) website.

## Overview

The contract period analyzed in this project spans from **April 17, 2024**, to **April 16, 2025**. During this period, MITRE received **$28,967,283.11** from CISA (Cybersecurity and Infrastructure Security Agency) to manage the CVE Program.

### Key Findings

- **Cost Per CVE Published During the Contract Period**:  
  MITRE received **$664.01** for each of the **43,625** CVEs published during the contract period.

- **Overall Cost Per CVE in the Database**:  
  MITRE received **$99.60** for each of the **290,834** CVEs in the CVE database during the contract period.

## Data Source

## Data Source

The data used in this analysis is sourced from the [CVE List V5 GitHub repository](https://github.com/CVEProject/cvelistV5). This repository contains JSON files with CVE records, organized by year. These files are processed to extract relevant metadata, including publication dates, CVSS scores, and affected products.

To ensure the data is up-to-date, the repository is cloned or updated programmatically using a sparse checkout to download only the necessary files. The process includes:

1. **Cloning the Repository**: If the local repository does not exist or is empty, the script clones the CVE List V5 repository with a sparse checkout to download only the `cves/` folder.
2. **Updating the Repository**: If the repository already exists, the script pulls the latest changes to ensure the data is current.
3. **Processing Files**: The JSON files in the `cves/` folder are iterated over and processed to extract the required information.

For more details, refer to the `Data_Download.ipynb` file in this repository.

The contract details can be found at the following link:  
[Contract Link](https://www.usaspending.gov/award/CONT_AWD_70RCSJ23FR0000015_7001_70RSAT20D00000001_7001)

## Repository Contents

## Repository Contents

- **`CVE_Cost.ipynb`**: The main Jupyter Notebook that calculates the cost of managing and maintaining the CVE Program.
- **`Data_Download.ipynb`**: A Jupyter Notebook that automates the process of downloading and updating CVE data from the CVE List V5 GitHub repository using a sparse checkout.
- **`overall_cna.csv`**: A CSV file summarizing the cost per CNA (CVE Numbering Authority) for all CVEs in the database.
- **`contract_period_cna.csv`**: A CSV file summarizing the cost per CNA for CVEs published during the contract period.
- **`CVE/`**: A directory containing JSON files with CVE data, organized by year.

## Requirements

To run the notebook, you need the following Python packages:

- `pandas`
- `matplotlib`
- `datetime`
- `os`
- `json`
- `re`

Install the required packages using the following command:

```bash
pip install -r requirements.txt 
```

## Usage
Clone the repository:

```bash
git clone https://github.com/your-username/CostOfCVE.git
cd CostOfCVE
```

Install the required dependencies:
```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook:
```bash
jupyter notebook CVE_Cost.ipynb
```

Run the notebook cells to perform the analysis.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
MITRE Corporation for managing the CVE Program.
CISA for funding the CVE Program.
USAspending.gov for providing publicly accessible contract data.