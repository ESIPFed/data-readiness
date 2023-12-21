## About the checklist

The checklist is developed using the 2019 draft readiness matrix developed by the Office of 
Science and Technology Policy Subcommittee on Open Science as a basis. The checklist has been 
improved based on further research and user feedback. Definitions for some concepts are listed
at the end of this document. This checklist is developed through a collaboration of ESIP Data 
Readiness Cluster members include representatives from NOAA, NASA, USGS, and other organizations.
The checklist will be updated periodically to reflect community feedback.

### How to use the checklist  

Ideally for AI-ready assessment, a dataset should be defined as the minimum measurable bundle 
(i.e., a physical parameter/variable of observational datasets or model simulations). The 
assessment at this scale will enable better integration of data from different sources for research
and development. However, it can be an intensive process for manual assessment without automation. 
Therefore, we recommend current assessments be done on the data file level. If the dataset has different 
versions, the checklist should be applied to each dataset type (e.g. raw, derived).

### How to cite this checklist:
> Information to be added after DOI is created by ESIP.

### History
**Version**: 1.0;  
**Last updated**: June 21, 2023.

---

## General Information
- Link to the dataset landing page (_questions below could be automatically filled from the landing page in the future_)
  - Name of the dataset
  - The current version of the dataset
  - Point of contact for the dataset
  - When was the dataset originally published?
- Is this raw data or a derived/processed data product? _Raw/Derived_
- Is this observational data, simulation/model output, or synthetic data? _Observed/Modeled/Synthetic_ 
- Is the data single-source or aggregated from several sources? _Single-source/Aggregated_

## Data Quality
- Questions on timeliness:
  - Will the dataset be updated? _Yes, it will be updated. / No, it will not be updated_
  - If the data will be updated, how often will it be updated? [choose from]
    - Updated when new data are added. 
      - Choose the update frequency that best describes the dataset: _near-real-time (irregularly) /
        hourly or sub-hourly / daily or sub-daily / weekly / monthly / yearly / longer than a year_ 
      - Will there be different stages of the update (e.g., updated with preliminary data first and
        replaced by a later update of the full record)? _Yes/No/Not applicable._
        - If yes, what is the delay between different stages? [short answer]
    - Updated when a new version of the dataset is available. 
      - Should the new version of the dataset supersede the current version? _Yes / No / Others_
        - Provide an explanation for “Others”
- Questions on data completeness
  - Is there any documentation about the completeness of the dataset? _Yes / No_
    - If yes, link to the report/document
  - How complete is the dataset compared to the expected spatial coverage?
    _Complete / Partial / Unknown / Not applicable_
  - How complete is the dataset compared to the expected temporal coverage?
    _Complete / Partial / Unknown / Not applicable_
- Questions on data consistency
  - Is this dataset self-consistent in that its units, data types, and parameter names
    do not change over time and space? _Yes / No / Not applicable_
  - Is this dataset’s units, data types, and parameter names consistent with similar data
    collections? _Yes / No / Not applicable_
  - Are there processes to monitor for units, data types, and parameter consistency?
    _Yes / No / Not applicable_
    - If yes, what measures are taken? _Manual review / Automated review_
- Questions on data bias
  - Is there known bias in the dataset? _Yes / No_
    - If yes, provide more information
  - Have measures been taken to examine bias? _Yes / No_
    - If yes, what measures were used?
    - Is the bias metrological traceable? 
  - Is there reported bias in the data? _No known bias / Bias found and reported / No information available_
    - (optional) Link to the report/document on the bias
    - (optional) Link to tools available to reduce bias
    - (optional) Link to a bias-corrected or bias-reduced version of the dataset 
  - Is there quantitative information about data resolution in space and time? _Yes / No / Not applicable_
  - Are there published data quality procedures or reports? _Yes / No_ 
    - If there is published quality information, please provide the link to the information.
  - Is the provenance of the dataset tracked and documented? _Yes / No / Not applicable_
  - Are there checksums / other checks for data integrity? Yes / No / Not applicable
  - What is the size of the dataset? Depending on the resource, this might be total data volume,
    dimensionality, number of images, data files, table rows, image size, etc. _[Short Answer]_

## Data Documentation
- Does the dataset metadata follow a community/domain standard or convention? _Yes / No / Not applicable_
  - If the metadata follows a community/domain standard, which standard is it? _Select from a list [CF, …, TBD, others]_
  - Is the dataset metadata machine-readable? _Yes / No / Not applicable_
  - Does it include details on the spatial and temporal extent? _Yes / No / Not applicable_
- Is there a comprehensive data dictionary/codebook that describes what each element of
  the dataset means? parameters? _Yes / No / Not applicable_
  - Is the data dictionary standardized? _Yes / No / Not applicable_
  - Is the data dictionary machine-readable? _Yes / No / Not applicable_
  - Do the parameters follow a defined standard? _Yes / No / Not applicable_
    - If the parameters follow a defined standard, which standard it is?
  - Are parameters crosswalked in an ontology or common vocabulary (e.g. NIEM)? _Yes / No / Not applicable_
- Does the dataset have a unique persistent identifier, e.g. DOI?  _Yes, [supply identifier]  / No / Not applicable_
- Is there contact information for subject-matter experts? _Yes / No / Not applicable_
- Is there a mechanism for user feedback and suggestions? _Yes / No / Not applicable_
- Are there example codes/notebooks/toolkits available showing how the data can be used? _Yes / No / Not applicable_
- What is the license for the data? 
  - Pick from a list of data licenses + others + no official data license 
  - Is the license standardized and machine-readable (e.g. Creative Commons)?  _Yes / No / Not applicable_
- Has this dataset already been used in AI or ML activities? _Link to publications/reports._
- Are there recommendations on the intended use of the data, and uses that are not
  recommended? _Yes / No/ Not applicable_

## Data Access  
- What is/are the major file formats? _Pick from a list of common data formats/ “other” (choose all that apply)_ 
  - Is this format machine-readable? _Yes / No / Not applicable_ 
  - Is the data available in at least one open, non-proprietary format? _Yes / No / Not applicable_
  - Are there tools/services to support data format conversion? _Yes / No_
    - If so, provide the link to the tools/services
- Data delivery:
  - Does data access require authentication (e.g., a registered user account)? _Yes / No / Not applicable_
  - Can the file be accessed via direct file downloading or ordering?  _Yes / No / Not applicable_
  - Is there an Application Programming Interface (API) or web service to access the data?
    _Yes / No / Not applicable_
  - If there is an API, does the API follow an open standard protocol (e.g., OGC)? _Yes / No_
  - If there is an API, is there documentation for the API? _Yes / No_
    - If “Yes”, please provide a URL to the documentation.
  - Is the data available publicly via cloud services?  _Yes / No / Not applicable_
- For restricted data, have measures been taken to provide some access while still applying
   appropriate protection for privacy and security?  _Yes / No / Not Applicable_
  - Has the data been aggregated to reduce granularity?  _Yes / No / Not applicable_
  - Has the data been anonymized / de-identified? _Yes / No / Not applicable_
  - Is there secure access to the full dataset for authorized users?  _Yes / No / Not applicable_

## Data Preparation
- Have null values/gaps been filled? _Yes / No / Not applicable_
- Have outliers been identified? _Yes, tagged / Yes, removed / No / Not applicable_
- Is the data gridded (regularly sampled in time and space)? 
  - Options to choose from (choose all that apply): 
    - _Regularly gridded in space / Constant time-frequency /
      Regularly gridded in space and constant time-frequency / Not gridded / Not applicable_
  - If the data is gridded, was it transformed from a different original sampling?
    _Yes, from irregular sampling / Yes,  from a different regular sampling / No, this is the original sampling_
  - If the data is resampled from the original sampling, is the data also available at the original sampling?
    _Yes / No / Only available at request / Not applicable_
- Are there associated targets or labels for supervised learning techniques (i.e., can this be
  used as a training dataset for supervised learning techniques)? _Yes / No / Not applicable_
  - _If there are associated targets/labels, are community labeling standards implemented
    (e.g., STAC label extension, ESA AIREO specification, etc)?_
    - A list of label standards to choose from + “others” option

---
## Appendix - Definition of terms used in the checklist

### Quality
- Completeness: the breadth of a dataset compared to an ideal 100% completion (spatial, temporal,
  demographic, etc.); important in avoiding sampling bias
- Consistency: uniformity within the entire dataset or compared with similar data collections;
  for example, no changes in units or data types over time; the item measured against itself or its
   a counterpart in another dataset or database
- Bias: a systematic tilt in the dataset when compared to a reference, caused for example by
  instrumentation, incorrect data processing, unrepresentative sampling, or human error;
  the exact nature of bias and how it is measured will vary depending on the type of data and the
  research domain.
- Uncertainty: parameter, associated with the result of a measurement, that characterizes the dispersion
   of the values that could reasonably be attributed to the measurand.
- Timeliness: the speed of data release, compared to when an event occurred or measurements were made;
   requirements will vary depending on the timeframe of the phenomenon (e.g., severe thunderstorms vs.
   climate change, or disease outbreaks vs. life expectancy trends)
- Provenance: identification of the data sources, how it was processed, and who released it.
- Integrity: verification that the data remains unchanged from the original; aka data fixity.

### Documentation
- **Dataset Metadata**: complete information about the dataset: quality, provenance, location, time period, responsible parties, purpose, etc.
- **Data Dictionary/Codebook**: complete information about the individual variables / measures / parameters within a dataset: type, units, null value, etc.
- **Identifier**: a code or number that uniquely identifies a dataset
- **Ontology**: formalized definitions of concepts within a domain of knowledge, and the nature of the inter-relationships among those concepts

### Data Access
- **Formats**: standards that govern how information is stored in a computer file (e.g., CSV, JSON, GeoTIFF, etc.); different AI user communities will have different requirements, so the best practice is to provide several format options to meet the needs of multiple high priority user communities.
- **Delivery Options**: mechanisms for publishing open data for public use (e.g., direct file download, Application Programming Interface (API), cloud services, etc.); different AI user communities will have different requirements, so the best practice is to provide several delivery options to meet the needs of multiple high priority user communities.
- **License/Usage Rights**: information on who is allowed to use the data and for what purposes, including data sharing agreements, fees, etc.; some federal data needs to have restrictions and some will be fully open, so rights should be documented in detail
- **Security/Privacy**: protection of data that is restricted in some way (privacy, proprietary/business information, national security, etc.)

## References:
1. OSTP Subcommittee on Open Science (2019), Draft AI-ready data matrix.
   (This draft document is not an official publication of the committee and can be requested for reference.)
