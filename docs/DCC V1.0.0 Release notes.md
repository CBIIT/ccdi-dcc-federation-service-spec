# CCDI Data Node V1.0.0 Release Notes

The Childhood Cancer Data Initiative (CCDI) is excited to announce the inclusion of clinical and phenotypic information from CCDI-managed data sets as a new participating node (https://dcc.ccdi.cancer.gov/) within the Data Federation Resource (https://cbiit.github.io/ccdi-federation-api-aggregation/). This allows users to search for CCDI curated data in alignment with the existing Data Federation V1.2.0 specifications. 

### Considerations

The CCDI Data Node V1.0.0 provides harmonized values aligned with the Federation data model and does not reflect all CCDI-curated data. Future releases will expand support for additional clinical and phenotypic data searches and enable access to unharmonized data at individual endpoints. The following implementation considerations apply to the CCDI Data Node: 

- The CCDI-managed data is currently based on the CCDI Data model Version 3.1, which has been harmonized to the existing CCDI Data Federation Specification (V1.2.0) to ensure consistency across all participating nodes (see Metadata below).
- The File endpoint currently supports sequencing files.
- Diagnosis values incorporate terms from [ICD-0 3.2](http://www.iacr.com.fr/index.php?Itemid=577), [WHO Pediatric Tumor](https://publications.iarc.who.int/Book-And-Report-Series/Who-Classification-Of-Tumours/Paediatric-Tumours-2023) and [Cancer Classifications for Kids](https://docs.stjude.cloud/cc4k).
- The [Uberon](https://www.ebi.ac.uk/ols4/ontologies/uberon) ontology was leveraged for anatomical site representation.
- PDX models and their sequencing data will be supported in a future release.
- Gateways, which provide additional information to define requirements for accessing a particular set of data, have not been implemented for this release.

  
### Metadata
Metadata (clinical, phenotypic, and administrative) has been harmonized to Common Data Elements (CDEs) registered in the Cancer Data Standards Registry and Repository ([caDSR](https://cadsr.cancer.gov)):  

| Subject (Participant)  | Sample                          | Study and File                      |
|------------------------|---------------------------------|-------------------------------------|
| Sex ([6343385](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=6343385%20and%20ver_nr=1))          | Sample ID ([15100774](https://cadsr.cancer.gov/onedata/Home.jsp))                     | Study Short Title ([11459812](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11459812%20and%20ver_nr=1))        | 
| Race ([2192199](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=2192199%20and%20ver_nr=1))         | Sample Tumor Status ([14688604](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=14688604%20and%20ver_nr=1))   | Study Name ([11459810](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11459810%20and%20ver_nr=1))               |
| Ethnicity ([2192217](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=2192217%20and%20ver_nr=2))    | Tumor Classification ([12922545](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=12922545%20and%20ver_nr=1)) | dbGaP phs Accession ([11524544](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11524544%20and%20ver_nr=1))      |                     
| Vital Status ([2847330](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=2847330%20and%20ver_nr=1)) | Tumor Grade ([11325685](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11325685%20and%20ver_nr=2))          | Institution ([12662779](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=12662779%20and%20ver_nr=1))              |
| Age at Vital Status ([12306025](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=12306025%20and%20ver_nr=1)) | Age at Diagnosis ([3225640](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=3225640%20and%20ver_nr=2))  | File Location ([11556141](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11556141%20and%20ver_nr=1))  |                    
| Subject ID ([6380049](https://cadsr.cancer.gov/onedata/Home.jsp))   | Age at Collection ([14473376](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=14473376%20and%20ver_nr=1))    |  File Description ([11280338](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11280338%20and%20ver_nr=1))        | 
| Associated Diagnoses   | Library Strategy ([6273393](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=6273393%20and%20ver_nr=1))      |  File Size ([11479876](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11479876%20and%20ver_nr=1))               |
|                        | Preservation Method ([8028962](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=8028962%20and%20ver_nr=2))   |  Md5sum ([11556150](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11556150%20and%20ver_nr=1))                  |
|                        | Disease Diagnosis (partially implemented) | File Type ([11416926](https://cadsr-stage.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11416926%20and%20ver_nr=2))      |  
|                        | Disease Phase ([12217251](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=12217251%20and%20ver_nr=1))  |                                           | 
|                        | ICD-O Morphology Code & Term ([11326261](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=11326261%20and%20ver_nr=1)) |                             | 
|                        | Library Source Material ([15235975](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=15235975%20and%20ver_nr=1)) |                                   |   
|                        | Library Selection Method ([6347743](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=6347743%20and%20ver_nr=2)) |                                  | 
|                        | Specimen Molecular Analyte Type ([15063661](https://cadsr.cancer.gov/onedata/dmdirect/NIH/NCI/CO/CDEDD?filter=CDEDD.ITEM_ID=15063661%20and%20ver_nr=1)) |                          |                                
|                        | Anatomical Site Uberon https://www.ebi.ac.uk/ols4/ontologies/uberon | |


### Filtered Search Capabilities

The CCDI Data Node supports filtered searches across harmonized fields. Each URL query parameter may appear at most once; if a parameter is duplicated, the server will arbitrarily select one of the provided values. URI query strings exceeding 2,048 bytes are not permitted. 

The table below provides an overview of the filter criteria supported: 

| Filter                      | CCDI Data Node V1.0.0 |
|-----------------------------|-----------|
| <div align="center"><strong>Subject</strong></div>||
| Sex                         |  ✔️       |
| Race                        | ✔️        |
| Ethnicity                   | ✔️        |
| Vital Status                | ✔️        |
| Identifiers                 | ✔️        |
| Age at Vital Status         | ✔️        |
| Depositions                 | ✔️        |
| <div align="center"><strong>Sample</strong></div>||    
| Sample ID                   | ✔️        | 
| Sample Tumor Status         | ✔️        |   
| Tissue Type                 | ✔️        | 
| Tumor Classification        | ✔️          |
| Tumor Grade                 |    ✔️        |   
| Age at Diagnosis            |    ✔️        |   
| Age at Collection           |    ✔️        |     
| Library Strategy            |    ✔️        |   
| Preservation Method         |   ✔️         |   
| Disease Diagnosis           |  ✔️          |   
| Disease Phase               |   ✔️         |   
| ICD-O Morphology Code and Term  |       |   
| Depositions                 | ✔️        |   
| Anatomical Site            | ✔️        |    
| Library Source Material     | ✔️        |   
| Specimen Molecular Analyte Type	| ✔️    |   
| Library Selection Method    |    ✔️        |   
| <div align="center"><strong>Study</strong></div>||      
| Institution                 | ✔️        |
| <div align="center"><strong>File</strong></div>| |  
| File Description            |   ✔️         | 
| File Size                   |   ✔️         | 
| Checksums MD5               |   ✔️         | 
| File Type                   |   ✔️         |
| Depositions                 |   ✔️         | 


### Additional Information

Read more about CCDI Federation API in the  [blog](https://cbiit.github.io/ccdi-federation-api/blog.html). We look forward to seeing the community continue to leverage this API and contribute to the ongoing enhancement of the CCDI Data Federation Resource. 

For questions related to CCDI Data Federation, please email [ncichildhoodcancerdatainitiative@mail.nih.gov](mailto:ncichildhoodcancerdatainitiative@mail.nih.gov).

