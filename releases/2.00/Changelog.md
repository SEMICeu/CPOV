# Core Public Organisation Changelog

## Introduction


This document describes the (major) changes to [the current version 1.0.0](https://github.com/SEMICeu/CPOV/tree/master/releases/1.00) of the Core Public Organisation Vocabulary (released in December 2016) for which a new version is being proposed ([version 2.0.0](https://semiceu.github.io/CPOV/releases/2.00/)). The list of changes results in the new version to be considered as a major release.

## Detailed changes from v1.0.0 to v2.0.0

The table below gives an overview of the classes (and their definitions) within both data models. Classes that are related are juxta-positioned.

**C** stands for changes in classes

**R** stands for changes in relationships

**P** stands for changes in properties

**D** stands for changes in data types

| Nr | Core Public Organisation Vocabulary v1.0.0 | Core Public Organisation Vocabulary v2.0.0 | Rationale | GitHub / Change |
| --- | --- | --- | --- | --- |
| D1 | **Contact point:** opening hours expects a structured literal value | **Contact point:** opening hours expects a literal value | Structured literal is not an existing data type. | Change |
| D2 | **Public organization:** alternative label expects a literal value | **Public organization:** alternative label expects a text value | Alignment with other Core Vocs. | Change |
| D3 | **Public organization:** description expects a literal value | **Public organization:** description expects a text value | Alignment with other Core Vocs. | Change |
| D4 | **Public organization:** identifier expects a literal (typed) value | **Public organization:** identifier expects a literal value | Alignment with other literal data types. | Change |
| D5 | **Public organization:** preferred label expects a literal value | **Public organization:** preferred label expects a text value | Alignment with other Core Vocs. | Change |
| P1 | **-** | **ChangeEvent.description: added property** | Give some content to the class. | Change |
| P2 | **-** | **ChangeEvent.startedAtTime: added property** | Give some content to the class. | Change |
| P3 | **-** | **ChangeEvent.endedAtTime: added property** | Give some content to the class. | Change |
| D6 | **PublicOrganization.identifier: Literal** | **PublicOrganization.identifier: Identifier** | Alignment with other Core Vocabularies. | Change |

## Changes since April 2021 

### Terms

| Nr | Core Public Organisation Vocabulary v2.0.0 2021  | Core Public Organisation Vocabulary v2.0.0 2022 | Rationale                                                   | GitHub/Change                                                                                                              |
| -- | ------------------------------------------------ | ----------------------------------------------- | ----------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| C1 | cpsv: FormalFramework                             | CCCEV: ReferenceFramework                        | Replaced by more generic framework                          | [https://github.com/SEMICeu/CPOV/issues/5](https://github.com/SEMICeu/CPOV/issues/5)                                       |
| C2 | FoundationEvent                                   | \-                                               | Removed as subclass of ChangeEvent                          | [https://github.com/SEMICeu/CPOV/issues/9](https://github.com/SEMICeu/CPOV/issues/9)                                       |
| C3 | skos: Concept                                     | \-                                               | made it implicit                                            |                                                                                                                            |
| C4 | schema: ImageObject                               | CoreVocabulary: ImageObject                      | replaced [schema.org](http://schema.org/) with cv namespace | [https://github.com/SEMICeu/CPOV/issues/10](https://github.com/SEMICeu/CPOV/issues/10)                                     |
| C5 | schema: ContactPoint                              | CoreVocabulary: ContactPoint                     | replaced [schema.org](http://schema.org/) with cv namespace | [https://github.com/SEMICeu/CPOV/issues/10](https://github.com/SEMICeu/CPOV/issues/10)                                     |
| C6 | schema: OpeningHoursSpecification                 | CoreVocabulary: OpeningHoursSpecification        | replaced [schema.org](http://schema.org/) with cv namespace | [https://github.com/SEMICeu/CPOV/issues/10](https://github.com/SEMICeu/CPOV/issues/10)                                     |
| C7 | CoreLocation: Geometry                            | \-                                               | Geometry is not related to AdministrativeTerritorialUnit    | [https://github.com/SEMICeu/CPOV/issues/7](https://github.com/SEMICeu/CPOV/issues/7)                                       |
| C8 | AdministrativeTerritorialUnits                    | AdministrativeTerritorialUnit                    | made it singular as per definitions rule                    | [https://github.com/SEMICeu/CPOV/issues/7](https://github.com/SEMICeu/CPOV/issues/7)                                       |
| R1 | PublicOrganisation.classification: Concept        | PublicOrganisation.classification                | made it implicit                                            |                                                                                                                            |
| R2 | PublicOrganisation.purpose: Concept               | PublicOrganisation.purpose                       | made it implicit                                            |                                                                                                                            |
| R3 | AdministrativeTerritorialUnits.geometry: Geometry | \-                                               | Geometry is not related to AdministrativeTerritorialUnit    | [https://github.com/SEMICeu/CPOV/issues/7](https://github.com/SEMICeu/CPOV/issues/7)                                       |
| P1 | Identifier.issuingAuthority                       | Identifier.issuingAuthorityName                  | Better property readability                                 | [https://github.com/SEMICeu/Core-Person-Vocabulary/issues/14](https://github.com/SEMICeu/Core-Person-Vocabulary/issues/14) |
| P2 | Identifier.identifier                             | Identifier.notation                              | to better distinguish it from the identifier itself         |                                                                                                                            |
| P3 | Identifier.issuingAuthorityURI                    | Identifier.issuingAuthorityURI: Agent            | the range of the property has been made more generic        |                                                                                                                            |
| D1 | Identifier.dateOfIssue: DateTime                  | Identifier.dateOfIssue: Date                     | the property is more generic                                |

### Definitions

Changes in definitions are registered in [this file](Changelog_definitions.md)