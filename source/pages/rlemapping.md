---
title: RLE Mapping
layout: default
active: guidance
topofpage: true
r4: http://hl7.org/fhir/R4/
us_r4: http://hl7.org/fhir/us/core/
---

This section describs the key Accuracy and Authenticity mapping requirements common to all Skin Wound Assessment actors used in this guide.

The conformance verbs used are defined in [FHIR Conformance Rules].

---

<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
**Contents**

* Do not remove this line (it will not be displayed)
{:toc}

---

<!-- end TOC -->

## Record Lifecycle Event Metadata Mapping

<br />

### AuditEvent Mapping

AuditEvent mapping goes here - table of AuditEvent data elements and the mapping to their data sources

<br />

### Provenance Mapping

Provenance mapping goes here
* [US Core Basic Provenance Guidance (R4)]
* [US Core Provenance (R4)]
* Table of Provenance data elements and the mapping to their data sources
  * Baseline mappings from [US Core Basic Provenance Guidance (R4)]

**Key Provenance elements:**

Element | Required | Must Support |Optional| FHIR Element|
---|---|---|---|---
Target | Resource Provenance <br>record supports | | | Provenance.target
Timestamp | Date | | Time with timezone offset | Provenance.recorded
Author | | Name<br>Identifier | NPI recommended, additional identifiers allowed| Provenance.agent.who
Author Organization | | Name<br>Identifier  | NPI recommended, additional identifiers allowed |Provenance.agent.onBehalfOf
Transmitter | | Name<br>Identifier | NPI recommended, additional identifiers allowed| Provenance.agent.who
Transmitter Organization | | Name<br>Identifier  | NPI recommended, additional identifiers allowed |Provenance.agent.onBehalfOf
{: .grid}

  * Additional mapping(s) per Skin Wound Assessment IG requirements against [FHIR Record Lifecycle Events Implementation Guide (R4)]

**Overlapping and Additional RLE Provenance elements:**

Element | Required | Must Support |Optional| FHIR Element| RLE Item|
---|---|---|---|---
Target | Resource Provenance <br>record supports | | | Provenance.target| **Originate/Retain Originate and Retain Record Entry (cc10)**
Period | Date Range | | Time with timezone offset | Provenance.occurredPeriod| **Evidence of Record Entry Originate/Retain Event (cc10)**
Timestamp | Date | | Time with timezone offset | Provenance.recorded| **Evidence of Record Entry Originate/Retain Event (cc11)**
Author | | Name<br>Identifier | NPI recommended, additional identifiers allowed| Provenance.agent.who| **Evidence of Record Entry Originate/Retain Event (cc4)**
Author Organization | | Name<br>Identifier  | NPI recommended, additional identifiers allowed |Provenance.agent.onBehalfOf| **Evidence of Record Entry Originate/Retain Event (cc4)**
Transmitter | | Name<br>Identifier | NPI recommended, additional identifiers allowed| Provenance.agent.who| **Evidence of Record Entry Originate/Retain Event (cc7)**
Transmitter Organization | | Name<br>Identifier  | NPI recommended, additional identifiers allowed |Provenance.agent.onBehalfOf| **Evidence of Record Entry Originate/Retain Event (cc7)**
{: .grid}

---

{% include link-list.md %}

