|    Term    |  	Description     |
|------------|--------------------|
|Archival Creator|Organisation unit or individual that creates records and/or manages records during their active use. 
|Archival Information Package (AIP)|An information package, consisting of the Content Information and the associated Preservation Description Information (PDI), which is preserved within an Open Archival Information System (OAIS).|
|Cardinality|The term describes the possible number of occurrences for elements in a set. The numbers have the following meanings:|
||(1..1) – in each set, there is exactly 1 such element present|
||(0..1) – the set can contain from 0 to 1 of such elements|
||(1..n) – the set contains at least one element|
||(0..n) – the set can contain up to n of such elements, but it is not mandatory|
||(0..0) – the element is prohibited to use.| 
|Case or Patient Case|Type of component consisting of a set of objects and/or sub-cases. This is represented in the specification as a directory that sits within the data directory of a representation (which in this case is a Patient’s Medical Record). A Case is an aggregation of individual records related to one patient and which are related in a way that is defined by national standards, guidance or local practice. A Patient’s Medical Record will consist of multiple individual thematic Cases which may be concerned with particular medical conditions, periods or treatments.|
|Central Health Archive|An organisation within a national or regional jurisdiction with a (usually legal) remit to create an archive of Patient Medical Records for people who have received primary or secondary healthcare in the jurisdiction. The Central Health Archive will be populated with Patient Medical Records from multiple healthcare providers in the jurisdiction, which will be drawn from Local Patient Health Archives (e.g. a hospital archive).|
|Component|	In this standard: meaningful, logically delimited, and uniquely identifiable information that may be subject to treatment in manual and/or automated processes. This standard operates with four generic types of components: Case, Document, Data File and Byte Stream.|
|Complete Patient Medical Record|The sum of the submissions of patient Records made for an individual.|
|Content Data Object|The Data Object, that together with associated Representation Information comprises the Content Informartion (Source OAISA – ISO 14721:2012).|
|Content Information|A set of information that is the original target of preservation or includes part or all of that information. It is an Information Object composed of its Content Data Object and its Representation Information. (Source OAIS – ISO 14721:2012).|
|Data File|A component which contains data and has an associated MIME file type.  A Data File can encapsulate multiple bit streams and metadata according to a standard such as a DICOM but must have a recognised MIME file type. A Data File may comprise one or more subsidiary Byte Streams; for example, an MP4 file might contain separate audio and video streams, each of which has its own associated metadata.| 
|Death Register|National system which records deaths within the jurisdiction.|
|Dissemenation Information Package (DIP)|Information Package, derived from one or more AIPs and sent by Archives to the Consumer in response to a request to the OAIS.|
|Document|A single or group of related Data Files with common metadata. For example, a Document may consist of a PDF file together with associated attachments or a word file with a separate image signature sheet. A document can be considered to be an entity that is approved/signed as a whole by a practitioner.|
|General EMR System|Electronic Medical Record system intended for documentation of all forms of healthcare. Note: large scale healthcare providers may have a main general-purpose EMR system but can also have a number of distributed general-purpose EMR systems serving parts of the organisation that operate as separate sub-services.|
|Healthcare Provider|An organisation providing primary or secondary healthcare. Can be general in scope or specialised, public or private.|
|Information Package|A logical container composed of optional Content Information and optional associated Preservation Description Information used to delimit and identify the Content Information and Package Description information used to facilitate searches for the Content Information.|
|Internal Archival|Long Term Preservation guidelines	This type of guideline can have different names depending on the creator. Generally, archives specify technical guidelines and/or regulations for formats, specifying what they will accept and maintain for the long term/ Depending on the archive and available technical resources, the criteria for the selected formats can differ from archive to archive.|
|Level|The level of requirements of the element following RFC 2119 http://www.ietf.org/rfc/rfc2119.txt.|
||MUST – this means that the definition is an absolute requirement|
||SHOULD – this means that in particular circumstances, valid reasons may exist to ignore the requirement, but the full implications must be understood and carefully weighed before choosing a different course.
||MUST NOT – this means that the prohibition described in the requirement is an absolute prohibition of the use of the element.|
||SHOULD NOT – this means that in particular circumstances, violating the prohibition described in the requirement is acceptable or even useful, but the full implications should be understood and the case carefully weighed before doing so. The requirement text should clarify such circumstances.|
||MAY – means that a requirement is entirely optional.|
|Local Patient Health Archive|An archive of physical or electronic Patient Medical Records within a Healthcare Provider or group of Healthcare Providers. A Patient Medical Record will normally be expected to be transferred to an archive either when the patient is known to have died, or after a number of years have passed since its creation that exceeds normal life expectancy.|
|Open Archival Information System (OAIS)|An Archive consisting of an organisation, which may be part of a larger organisation, of people and systems, that has accepted the responsibility to preserve information and make it available for a Designated Community. It meets a set of responsibilities that allows an OAIS Archive to be distinguished from other uses of the term ‘Archive’. 
|Patient|A person who has received medical treatment.|
|Patient Clinical Information|Structured patient clinical data related to Cases such as diagnoses, procedures, medication, allergies, etc.
|Patient Manifest|Structured manifest containing at minimum the full names of the each Patient who has records in the package together with a unique ID (such as a social security or health number).|
|Patient Medical Record|Collection or compilation of recorded information about a patient in connection with healthcare. Note: a Patient Medical Record may contain information in digital form and/or information recorded on other types of media such as paper or film. For the purposes of this specification, Patient Medical Records are assumed to be digital where the content may be born digital and/or digitised from physical records.|
|Patient Medical Record Extraction|Extract from a Local Health Archive for the purposes of handing off to the Central Health Archive. All Patient Medical Record Extractions should be under a Submission Agreement.|
|Patient Administrative Information|Demographics and other administrative information about an individual receiving care or other health-related services. For example, as can be described using the resource FHIR.Patient. Information will include but not be limited to name, patient ID(s), administrative gender, date of birth, date of death, address(es).
|RDBMS|Relational Database Management System
|Representation|A Representation within an Information Package contains archival data. If an Information Package contains the same data in two or more different formats (i.e. an original and a long term preservation format) or in different types of organisations (arrangements), the are placed within two or more separate Representations within the Representations folder of the Information Package of the Information Package.|
|Representation Information|The Representation Information must enable or allow the re-creation of the significant properties of the original data object.
|Specialised EMR System|Electronic Medical Record system specially adapted for documentation of a type of specialised healthcare or integrated with a specialised device. Examples: food/maternity system, gastrosystem, laboratory system, etc.|
|Standardised Machine- readable Documentation|A standardised machine-readable document is a document whose content can be readily processed by computers and is based on a commonly accepted standard. Such documents are distinguished from machine-readable data by virtue of having sufficient structure to provide the necessary context to support the business processes for which they are created.|
|Sub-case|Type of component consisting of a set of thematically related Data Files which are also related to a Case. Sub-cases are represented in the specification as folders that sit within a Case.|
|Submission Agreement|The agreement reached between an archive and the submission producer that specifies a submission format (eHealth1 CITS), and any other arrangements needed, for the data submission session. Any special conditions on patient confidentiality could be specified in the submission agreement.|
|Submission Information Package (SIP)|An Information Package that is delivered by the Producer to the OAIS for use in the construction or update of one or more AIPs and/or the associated Descriptive Information.|
|Submitting Organisation|Name of the organisation submitting the package to the archive.|