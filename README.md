# FAIR Dataset: MomCare Program (2017-2023)

Welcome to the GitHub repository for the **MomCare Data**. This dataset follows the FAIR (Findable, Accessible, Interoperable, and Reusable) data principles to support transparency, reproducibility, and reuse in research.

## Overview

**Description**:  
This dataset includes billing and survey data of approximately 30,000 women who enrolled in the PharmAccess MomCare program across urban and rural areas of Kenya since the start of 2017 until the end of 2023.

 **Domain**: Health  
 **Geographic Scope**: Kenya: Nairobi, Kisumu, and Kakamega county 
 **Time Period**: 2017 - 2023
 **Data Type**: Claims and survey data 
 **Data Model**: Based on [FHIR International Patient Summary](http://hl7.org/fhir/uv/ips/ImplementationGuide/hl7.fhir.uv.ips) 


## Repository Structure

### 1. Standardized Metadata Model 
In our use-case, the MomCare (meta)data will be registered on the [eLwazi Metadata Catalogue](https://catalog.elwazi.org/#/datasets), improving findability and accessibility for meta-analysis. However, eLwazi’s metadata fields are tailored to its user community and lack highly machine-actionable export options. 

We propose a standardized metadata model, as an extension of FHIR-based datasets, to specify a minimal set of metadata requirements. 
The model extends the DCAT framework by incorporating dataset descriptors relevant to eLwazi users, such as Sample Size and Countries, while integrating version, format, and storage details more explicitly than DCAT:
!()[./FAIRwithFHIR_MomCare_metadata.png]

To enhance machine-actionability, we also generated an RDF-version of this metadata model. This metadata can be found [here](./metadata.ttl). 

### 2. Data Access 

## Data Access

More information about the data can be accessed via the [eLwazi Metadata Catalogue](https://catalog.elwazi.org/#/datasets) and found [here](./metadata.ttl). 

**Anonymized data** 

In order to clarify for what purposes the data can be reused, the license conditions need to be findable and within the metadata. The [CC BY-SA 4.0 Creative Commons License](https://creativecommons.org/licenses/by-sa/4.0/) was attributed to the data, allowing free sharing and adaptation of the data under the terms of attribution (giving appropriate credit to the licensor) and sharing alike (distribution under the same license as the original).

The anonymized MomCare dataset adheres to these Creative Commons reuse conditions, which are also captured in the metadata. The anonymized data can be retrieved via [duckdb](./duckdb.md).

**Data Access Request** 

Access to the full dataset is restricted due to personal data content. Users must submit an access request to the data access committee, following the protocol described [here](./dataaccess.md). 

### 3. Semantic Interoperability

The FHIR standard is set-up to drive data interoperability and re-use within the FHIR community. We propose that the semantic interoperability can be improved by using the OnTop tooling. 

This use of the docker is described [here](./ontop.md)