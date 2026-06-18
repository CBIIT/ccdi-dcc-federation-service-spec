**CCDI Data Node V1.1.0 Release Notes**

The Childhood Cancer Data Initiative (CCDI) is announcing the next
release of the CCDI-managed data sets within the Data Federation
Resource
([<u>https://cbiit.github.io/ccdi-federation-api-aggregation/</u>](https://cbiit.github.io/ccdi-federation-api-aggregation/)).
This allows users to search for CCDI curated data in alignment with the
recently released Data Federation V1.3.0 specification which adds
diagnosis category to existing endpoints as follows:

- **Subject**: the `/subject` and `/subject-diagnosis` endpoints entities
  now can provide `associated_diagnosis_categories` data.

- **Sample**: the `/sample` and `/sample-diagnosis` endpoints entities now
  can provide `diagnosis_category` data.

- **Sample Experimental**: the `/sample` and `/sample-diagnosis` endpoints
  now support a `diagnosis_category` search parameter.

- **Subject Experimental**: the `/subject-diagnosis` endpoint now supports
  an `associated_diagnosis_categories` search parameter.

- **Metadata Endpoints (Subject and Sample)**: Updated to support
  linking of new information related to diagnosis category.

In addition, a new file type, methylation array, was added to the
existing **File Endpoint** to provide additional data in the API.

**Considerations**

The following implementation considerations apply to the CCDI Data Node:

- The CCDI Data node includes both harmonized and unharmonized values
  for Diagnosis Category

  - Harmonized values align with the API specification [CDE
    16607972 v1.0](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=16607972%20and%20ver_nr=1)
    Diagnosis Pediatric Oncology Grouping Category.

  - Unharmonized values for diagnosis category map to C[DE
    6161017 v1.0](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=6161017%20and%20ver_nr=1)
    ICD-O Disease Diagnosis Category.

- For the CCDI DCC node V1.1.0, there are more unharmonized values than
  harmonized in the API response.

**Additional Information**

Read more about CCDI Federation API in
the [<u>documentation</u>](https://cbiit.github.io/ccdi-federation-api/).
We look forward to seeing the community continue to leverage this API
and contribute to the ongoing enhancement of the CCDI Data Federation
Resource.

For questions related to CCDI Data Federation, please
email [<u>ncichildhoodcancerdatainitiative@mail.nih.gov</u>](mailto:ncichildhoodcancerdatainitiative@mail.nih.gov).
