---
title: Use Cases
layout: default
active: usecases
topofpage: true
r4: http://hl7.org/fhir/R4/
us_r4: http://hl7.org/fhir/us/core/
---

Please refer to each Use Case definition page for specific guidance:

1. [Use Case - Originate and Retain (null), then Amend (populate with clinical content)](usecase-originate.html): FHIR Record Lifecycle Event (RLE) Originate and Retain, and Amend in relation to the initial creation of the Wound Assessment Template (WAT) data as empty templates and then fully populated instances in an EHR actor system
  * This represents the first trial definition of incorporating the RLE Originate and Retain event and RLE Amend event into the the WAT data creation. This is the simplest way for the local system to demonstrate that the "populate with clinical content" step began from an "all null clinical content" state. This also establishes that the null-state template may pre-exist on the local system for any interval (seconds to years) prior to its "Amend" to add an instance of assessment.
  * For future work, we may identify the complexity of demonstrating that the null-state version could be empty also of patient demographics, thus the null state could be used as the initial state for all subsequent patient-specific captures as Amend events to the all-null original.


2. [Use Case - Receive and Retain](usecase-receive.html): FHIR Record Lifecycle Event (RLE) Receive and Retain in relation to the sending of Wound Assessment Template (WAT) data from an EHR actor system to a Wound Assessement Registry (WAR) actor system

3. [Use Case - Search](usecase-search.html): Query and retrieval of the Wound Assessment Template (WAT) data from either an EHR actor system or Wound Assessement Registry (WAR) actor system

---

{% include link-list.md %}
