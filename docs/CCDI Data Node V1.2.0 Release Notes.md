# CCDI Data Node V1.2.0 Release Notes
_Jagu, Subhashini (NIH/NCI)_

The Childhood Cancer Data Initiative (CCDI) is announcing the next
release of the CCDI-managed data sets within the Data Federation
Resource
([<u>https://cbiit.github.io/ccdi-federation-api-aggregation/</u>](https://cbiit.github.io/ccdi-federation-api-aggregation/)).

This change supports the CCDI V1.0 Data model and aligns with the
existing Data Federation API Specification (V1.3.0). This release
increases the available data to 45 studies.

Apart from changes to syntax for unharmonized values, technical changes
are driven by mapping the new data model to the existing API
specification.

**Subject and Subject Experimental**

- Aligns syntax for unharmonized values to the API specification
  for unharmonized.associated_diagnosis_categories
  
- Mapping changes for sex

- String to list for race, ethnicity, associated  properties in
  diagnosis nodes

**Sample and Sample Experimental**

- Mapping changes for API tumor classification to DCC Diagnosis Disease Extent Type (tumor_spatial_extent), preservation method, and diagnosis category

- Aligns syntax for unharmonized values with the for unharmonized.diagnosis_category

- Additional transformations for diagnosis category

- String to list changes for diagnosis, participant, sample exposure,
  medical history, treatment response, synonym study, radiology file

**File Endpoint**

- Mapping changes for ID to GUID
- Mapping changes for file types

## Additional Information

Read more about CCDI Federation API in
the [documentation](https://cbiit.github.io/ccdi-federation-api/).
We look forward to seeing the community continue to leverage this API
and contribute to the ongoing enhancement of the CCDI Data Federation
Resource.

For questions related to CCDI Data Federation, please
email [ncichildhoodcancerdatainitiative@mail.nih.gov](mailto:ncichildhoodcancerdatainitiative@mail.nih.gov).
