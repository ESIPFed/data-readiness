Note that some of these factors came from the draft readiness matrix developed by the Office of 
Science and Technology Policy Subcommittee on Open Science, and some have been added based on 
further research. Definitions for some concepts are listed at the end of this document. 
This checklist is developed through a collaboration of ESIP Data Readiness Cluster members 
including representatives from NOAA, NASA, USGS, and other organizations. The checklist will 
be updated periodically to reflect community feedback.

**Version**: 0.2;  **Last updated**: April 1, 2022.

How to cite this checklist:
> ESIP Data Readiness Cluster (2022): Checklist to Examine AI-readiness for Open Environmental Datasets. 
> ESIP. Online resource. https://doi.org/10.6084/m9.figshare.19983722.v1

---

## Data Preparation
- Have null values/gaps been filled? _Yes/No/Not applicable_
- Have outliers been identified? _Yes, tagged/Yes, removed/No/Not applicable_
- Is the data single-source or aggregated from several sources? _Single/Aggregated_
- Has the data been gridded (regularized in space and time) or is it in the originally sampled resolution? _Gridded/Not gridded/Not applicable_
- Have targets been identified and labeled (i.e. can this be used as a training dataset for supervised learning techniques)? _Yes/No/Not applicable_

## Data Quality
- Have measures been taken to ensure completeness? _Yes/No/Not applicable_
- Are there automated processes to monitor consistency? _Yes/No/Not applicable_
- Have measures been taken to reduce bias? _Yes/No/Not applicable_
- What is the timeliness of the data? _Near real-time, 1 week, 1 month, 1 year, more than 1 year_
- Is there a difference between raw near real-time access vs fully quality-controlled data that has an additional delay? _Yes/No/Not applicable_
- Are there quantitative measures of uncertainty? _Yes/No/Not applicable_
- Is there quantitative information about data resolution in space and time? _Yes/No/Not applicable_
- Are there published data quality procedures or reports? _Link to reports._
- Is the provenance tracked and documented? _Yes/No/Not applicable_
- Are there checksums / other checks for data integrity? _Yes/No/Not applicable_
- How big is the dataset? Depending on the resource, this might be total data volume, dimensionality, number of images, data files, table rows, image size, etc. (Short Answer)
- Is this essentially raw data or a derived/processed data product? _Raw/Derived_
- Is this observational data or simulation/model output? _Observed/modeled_
- Has the data been peer-reviewed? _Yes/No/Not applicable_
- Has it been down-sampled to reduce resolution, or is it raw? If so, are the raw data available?

## Data Documentation
- Does the dataset have metadata? _Yes/No/Not applicable_
  - Is the dataset metadata standardized? _Yes/No/Not applicable_
  - Is the dataset metadata machine-readable? _Yes/No/Not applicable_
  - Does it include details on the spatial and temporal extent? _Yes/No/Not applicable_
- Is there a comprehensive data dictionary/codebook to describe parameters? _Yes/No/Not applicable_
  - Is the data dictionary standardized? _Yes/No/Not applicable_
  - Is the data dictionary machine-readable? _Yes/No/Not applicable_
  - Do the parameters follow a defined standard? _Yes/No/Not applicable_
  - Are parameters crosswalked in an ontology or common vocabulary (e.g. NIEM)? _Yes/No/Not applicable_
- Does the dataset have a unique persistent identifier, e.g. DOI? _Yes/No/Not applicable_
- Is there contact information for subject-matter experts? _Yes/No/Not applicable_
- Is there a mechanism for user feedback and suggestions? _Yes/No/Not applicable_
- Are there example codes / notebooks / toolkits available showing how the data can be used? _Yes/No/Not applicable_
- Is there a clear data license? _Yes/No/Not applicable
  - Is the license standardized and machine-readable (e.g. Creative Commons)? _Yes/No/Not applicable_
- Has this dataset already been used in AI or ML activities? _Link to publications/reports._
- Are there recommendations on the intended use of the data, and uses that are not recommended? _Yes/No/Not applicable_

## Data Access
- What is the file format? Pick from list / “other” 
  - Is it machine-readable? Yes / No / Not applicable 
  - Is it available in at least one open, non-proprietary format? Yes / No / Not applicable
  - Is it available in several different file formats? Yes / No / Not applicable
- Data delivery:
  - Direct file download or ordering?  Yes / No/ Not applicable
  - Is there an API?  Yes / No/ Not applicable
    - Custom-developed or open, standard protocol? Custom / Standard
  - On the cloud?  Yes / No/ Not applicable
- For restricted data, have measures been taken to provide some access while still applying appropriate protection for privacy and security?  Yes / No / Not Applicable
  - Has the data been aggregated to reduce granularity?  Yes / No / Not applicable
  - Has the data been anonymized / de-identified?  Yes / No / Not applicable
  - Is there secure access to the full dataset for authorized users?  Yes / No / Not applicable

---
## Appendix - Definition of terms used in the checklist

### Data Quality
- **Completeness**: the breadth of a dataset compared to an ideal 100% completion (spatial, temporal, demographic, etc.); important in avoiding bias
- **Consistency**: uniformity within the entire dataset or compared with similar data collections; for example, no changes in units or data types over time; item measured against itself or its counterpart in another dataset or database
- **Bias**: a systematic tilt in the dataset, caused for example by instrumentation, incorrect data processing, unrepresentative sampling, or human error; the exact nature of bias and how it is measured will vary depending on the type of data and the research domain
- **Timeliness**: the speed of data release, compared to when an event occurred or measurements were made; requirements will vary depending on the timeframe of the phenomenon (e.g., severe thunderstorms vs. climate change, or disease outbreaks vs. life expectancy trends)
- **Provenance**: identification of the data sources, how it was processed, and who released it
- **Integrity**: verification that the data remains unchanged from the original; aka data fixity

### Data Documentation
- **Dataset Metadata**: complete information about the dataset: quality, provenance, location, time period, responsible parties, purpose, etc.
- **Data Dictionary/Codebook**: complete information about the individual variables / measures / parameters within a dataset: type, units, null value, etc.
- **Identifier**: a code or number that uniquely identifies a dataset
- **Ontology**: formalized definitions of concepts within a domain of knowledge, and the nature of the inter-relationships among those concepts

### Data Access
- **Formats**: standards that govern how information is stored in a computer file (e.g., CSV, JSON, GeoTIFF, etc.); different AI user communities will have different requirements, so the best practice is to provide several format options to meet the needs of multiple high priority user communities.
- **Delivery Options**: mechanisms for publishing open data for public use (e.g., direct file download, Application Programming Interface (API), cloud services, etc.); different AI user communities will have different requirements, so the best practice is to provide several delivery options to meet the needs of multiple high priority user communities.
- **License/Usage Rights**: information on who is allowed to use the data and for what purposes, including data sharing agreements, fees, etc.; some federal data needs to have restrictions and some will be fully open, so rights should be documented in detail
- **Security/Privacy**: protection of data that is restricted in some way (privacy, proprietary/business information, national security, etc.)

