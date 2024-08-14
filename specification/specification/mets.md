# 8 METS
<a name="section 8.1"><a/>
## 8.1 Use of METS in eHealth1
CSIP specifies that METS files be located at the root of the package folder structure (Root METS) and optionally in each of the representations within its respective root folder (Representation METS). 
<a name="section 8.2"><a/>
## 8.2 Root METS File
The root METS file must adhere to the requirements of the CSIP and Information Package specifications. In addition, there are specific requirements for the eHealth1 CITS, and in some cases, the level of the CSIP or package requirements have been increased (but never decreased).

### 8.2.1 Root METS root element
The eHealth1 CITS specification does not change or extend any of the requirements for the Root METS root element. Information is given below regarding the specific content type attributes to be used in an eHealth1 CITS.
### 8.2.2 Root METS header element (element metsHdr)
The following describes the differences in the package metsHdr element between CSIP, IP and the eHealth 1 CITS specification.
### 8.2.3 Root METS descriptive metadata section (element dmdSec)
The CSIP and IP specifications do not make any assumptions regarding the use of specific descriptive metadata schemas. The structure of the eHealth1 CITS is built on the concept of being patient-centric, and so a standardised metadata schema is preferred for Patient Administrative Information. The use of schemas such as ISO 13606 or HL7 FHIR is suggested but is not mandatory as local regulations and standards may be used.
### 8.2.4 Root METS administrative metadata section (element amdSec)
The eHealth1 CITS specification does not change or extend any of the requirements already defined by the CSIP or IP specifications’ administrative metadata section. The eHealth1 root METS document amdSec element SHOULD comply with the amdSec requirements in the CSIP profile. Note that in eHealth1, it is required that any rights or digital provenance metadata that is general to the package should be held within the root metadata folder and that any rights or digital provenance metadata that is specific to the data held in the representations should be held in the respective representation metadata folder.
### 8.2.5 Root METS file section (element fileSec)
The CSIP does not make the use of the METS fileSec element mandatory, but it is strongly recommended. In the eHEALTH CITS, the use of the METS fileSec element at the package level becomes mandatory, such as to reference the mets files within each representation.
### 8.2.6 Root METS structural map (element structMap)
The METS structural map element is the only mandatory element in the METS specification. It provides an overview of the components described in the METS document. It can also link the elements in the structure to associated content files and metadata. In the eHealth1 CITS, the package structMap describes the high-level structure of all the content in the package and links to at least one representation. 
s referenced from the package METS.xml via the <mptr> element, and hence the requirements for the structMap element within the package METS.xml (CSIP requirements CSIP80 to CSIP118) are unchanged. Because a representation is present, the need for a Content Division in the package METS.xml structMap is not required (CSIP101 to CSIP104 and CSIP109).
Implementers are welcome to define additional structural maps for their internal purposes by repeating the structMap element. The specific requirements for elements, sub-elements and attributes for eHealth1 CITS, which differ from the CSIP, are listed in the following table. 
<a name="section 8.3"><a/>
## 8.3 Representation METS
The representation METS files is used to describe the data structure as included in the data folder of the Representation  Medical Record) via the structMap element and to reference any additional descriptive metadata.
### 8.3.1 Representation METS root element
Particular notice is drawn to the specific requirements for a representation METS root element as described in the CSIP specification.
### 8.3.2 Representation METS header element (element metsHdr)
There are no requirements for a specific header element in the representation METS. The eHealth1 representation metsHdr element should comply with the metsHdr requirements in the SIP profile.
Note that the information contained in the representation header element relate specifically to the representation METS document.   
### 8.3.3 Representation METS descriptive metadata section (element dmdSec)
The Representation may contain additional descriptive metadata within the metadata/descriptive folder as described in the CSIP. It is recommended however that Patient Clinical Information related to the Patient Cases that can contain clinical information (diagnoses, conditions, procedures, allergies, family history, care plans) such as can be found in ISO 13606 or the HL7 FHIR Clinical Module  and that has been extracted from the source EMR system is included within each individual Patient Record in the repname/data folder, such as to simplify separation of Patient records into individual SIPs at the Archive. Use of metadata standards and codings (e.g. International Classification of Diseases ICD, https://www.who.int/classifications/icd/en/, Systematized Nomenclature of Medicine, SNOMED CT, www.snomed.org) is encouraged. Where used, references to the specific schemas os resources should be given together with relevant version information.
### 8.3.4 Representation METS administrative metadata section (element amdSec)
The administrative metadata section contains four sub-sections, each used to record different types of metadata for package content:
•	technical metadata (element techMD) records technical metadata;
•	rights metadata (element rightsMD) records intellectual property rights information;
•	source metadata (element sourceMD) records descriptive, technical or rights metadata for an analogue source for a digital library object; and
•	digital provenance metadata (element digiprovMD) records digital preservation information (e.g. audit information covering a digital library object’s life-cycle).

The CSIP only describes the use of the elements digiprovMD and rightsMD within the administrative metadata section of the METS.
The CSIP (and METS) categorises preservation metadata as administrative metadata, specifically Digital Provenance metadata (following the available guidelines published by the PREMIS EC guidelines: http://www.loc.gov/standards/premis/guidelines2017-premismets.pdf). Hence all preservation metadata should be referenced from a digiprovMD element within the amdSec.

The METS amdSec element should include references to all relevant metadata located in the folder “repname/metadata/preservation”. The package level METS.xml file should only reference package level preservation metadata. Representation level METS.xml files should only reference representation level preservation metadata.

In eHealth1, it is required that any rights or digital provenance metadata that is general to the package can be held within the root metadata folder and that any rights or digital provenance metadata that is specific to the data held in the representation should be held in the representation metadata folder.
The eHealth1 representation METS document amdSec element should comply with the requirements in the CSIP profile.
### 8.3.5 Representation METS structural map (structMap element)
The METS structural map element is the only mandatory element in the METS specification and is hence mandatory within the representation METS. The representation METS.xml is referenced from the package METS.xml via the <mptr> element, and hence the requirements for the structMap element within the package METS.xml (CSIP requirements CSIP80 to CSIP118) are unchanged. Because a representation is present, the need for a Content Division in the package METS.xml structMap is not required (CSIP101 to CSIP112 and CSIP 116, 118 and 119).
There MUST be one structural map present following the requirements of the CSIP.