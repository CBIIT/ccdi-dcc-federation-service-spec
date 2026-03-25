# CCDI Data Node V1.0.0 Release Notes

The Childhood Cancer Data Initiative (CCDI) is excited to announce the inclusion of clinical and phenotypic information from CCDI-managed data sets as a new participating node (https://dcc.ccdi.cancer.gov/) within the Data Federation Resource (https://cbiit.github.io/ccdi-federation-api-aggregation/). This allows users to search for CCDI curated data in alignment with the existing Data Federation V1.2.0 specifications. 

Metadata (clinical, phenotypic, and administrative) has been harmonized to Common Data Elements (CDEs) registered in the Cancer Data Standards Registry and Repository ([caDSR](https://cadsr.cancer.gov)). The CCDI Data Node V1.0.0 supports filtered searches across harmonized fields. 

### Considerations

The CCDI Data Node V1.0.0 provides harmonized values aligned with the Federation data model and does not reflect all CCDI-curated data. Future releases will expand support for additional clinical and phenotypic data searches and enable access to unharmonized data at individual endpoints. The following implementation considerations apply to the CCDI Data Node: 

- The CCDI-managed data is currently based on the CCDI Data Model Version 3.1.0, which has been harmonized to the existing CCDI Data Federation Specification (V1.2.0) to ensure consistency across all participating nodes.
- The File endpoint currently supports sequencing files.
- Diagnosis values incorporate terms from [ICD-0 3.2](http://www.iacr.com.fr/index.php?Itemid=577), [WHO Pediatric Tumor](https://publications.iarc.who.int/Book-And-Report-Series/Who-Classification-Of-Tumours/Paediatric-Tumours-2023) and [Cancer Classifications for Kids](https://docs.stjude.cloud/cc4k).
- The [Uberon](https://www.ebi.ac.uk/ols4/ontologies/uberon) ontology was leveraged for anatomical site representation.
- PDX models and their sequencing data will be supported in a future release.
- Gateways, which provide additional information to define requirements for accessing a particular set of data, have not been implemented for this release.

### Additional Information

Read more about CCDI Federation API in the  [documentation](https://cbiit.github.io/ccdi-federation-api/). We look forward to seeing the community continue to leverage this API and contribute to the ongoing enhancement of the CCDI Data Federation Resource. 

For questions related to CCDI Data Federation, please email [ncichildhoodcancerdatainitiative@mail.nih.gov](mailto:ncichildhoodcancerdatainitiative@mail.nih.gov).

