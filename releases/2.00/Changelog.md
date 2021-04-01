# Transition from Core Public Organisation v1.0.0 to v2.0.0

## Introduction

This document describes the (major) changes to [the current version 1.0.0](https://github.com/SEMICeu/CPOV/tree/master/releases/1.00) of the Core Public Organisation Vocabulary (released in December 2016) for which a new version is being proposed ([version 2.0.0](https://semiceu.github.io/CPOV/releases/2.00/)). The list of changes results in the new version to be considered as a major release.

## Detailed changes

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
