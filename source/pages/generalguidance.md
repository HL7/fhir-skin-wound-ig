---
title: General Guidance
layout: default
active: guidance
topofpage: true
r4: http://hl7.org/fhir/R4/
us_r4: http://hl7.org/fhir/us/core/
---

This section outlines important definitions and interpretations and requirements common to all Skin Wound Assessment actors used in this guide.
The conformance verbs used are defined in [FHIR Conformance Rules].

---

<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->
**Contents**

* Do not remove this line (it will not be displayed)
{:toc}

---

<!-- end TOC -->

## Use Case Guidance

The Use Case definitions represent descrete portions of functionality within a given EHR actor system and/or Wound Assessment Registry (WAR) actor system complete workflow in capturing Wound Assessment Template data. This specificity provides the implementer with a more focused representation of the needed functionality within their given system.

Please refer to each Use Case definition page for specific guidance:

1. [Use Case - Originate and Retain (null), then Amend (populate with clinical content)](usecase-originate.html): FHIR Record Lifecycle Event (RLE) Originate and Retain, and Amend in relation to the initial creation of the Wound Assessment Template (WAT) data as empty templates and then fully populated instances in an EHR actor system
  * This represents the first trial definition of incorporating the RLE Originate and Retain event and RLE Amend event into the the WAT data creation. This is the simplest way for the local system to demonstrate that the "populate with clinical content" step began from an "all null clinical content" state. This also establishes that the null-state template may pre-exist on the local system for any interval (seconds to years) prior to its "Amend" to add an instance of assessment.
  * For future work, we may identify the complexity of demonstrating that the null-state version could be empty also of patient demographics, thus the null state could be used as the initial state for all subsequent patient-specific captures as Amend events to the all-null original.


2. [Use Case - Receive and Retain](usecase-receive.html): FHIR Record Lifecycle Event (RLE) Receive and Retain in relation to the sending of Wound Assessment Template (WAT) data from an EHR actor system to a Wound Assessement Registry (WAR) actor system

3. [Use Case - Search](usecase-search.html): Query and retrieval of the Wound Assessment Template (WAT) data from either an EHR actor system or Wound Assessement Registry (WAR) actor system


## Record LifeCycle Events

Processing of the FHIR Record Lifecycle Events is defined as the capture of Conformance Criteria from each the following EHR FM R2 Record Infrastructure (RI) sections. The initial minimum required candidate Conformance Criteria are highlighted. Additional criteria may be processed by a system but will not be required at this time.

**a. Originate/Retain Originate and Retain Record Entry (Function RI.1.1.1)**
* i. (cc1)The system SHALL provide the ability to capture (originate) a Record Entry instance corresponding to an Action instance and context
* ii. (cc2) The system SHALL capture a unique instance identifier for each Record Entry.
* iii. (cc3) The system SHALL capture the signature event (e.g., digital signature) of the origination entry Author, binding signature to Record Entry content.
* iv. (cc4)The system SHALL provide the ability to capture both structured and unstructured content in Record Entries.
* v. (cc5) The The system SHALL provide the ability to capture Record Entries from information recorded during system downtime.
* vi. (cc6) The system SHOULD provide the ability to integrate Record Entries from Information recorded during system downtime.
* vii. (cc7) The system SHALL provide the ability to capture the date/time an Action was taken or data was collected if different than date/time of the Record Entry.
* viii. (cc8) The system SHOULD capture metadata that identifies the source of non-originated Record Entry (e.g., templated, copied, duplicated, or boilerplate information).
* ix.  (cc9) The system MAY provide the ability to tag unstructured Record Entry content to organize it according to need, for example, in a time-related fashion or by application-specific groups (such as photographs, handwritten notes, or auditory sounds), or by order of relative importance.
* <div id="publish-box">x. (cc10) The system SHALL capture and maintain a Record Entry encoded as a standards-based data object (e.g., HL7 Continuity of Care, other HL7 CDA R2 Document, ISO 13606 artifact).</div>
* xi. (cc11) The system MAY capture and maintain a standards-based data object to mirror (be duplicate and synchronous with) internal Record Entry representation.

**b. Evidence of Record Entry Originate/Retain Event (Function RI.1.1.1.1)**
* i. (cc1) The system SHALL audit each occurrence when a Record Entry is originated and retained.
* ii. (cc2) The system SHALL capture identity of the organization where Record Entry content is originated.
* iii. (cc3) The system SHALL capture identity of the patient who is subject of Record Entry content.
* <div id="publish-box">iv. (cc4) The system SHALL capture identity of the individual(s) who performed the Action documented in Record Entry content.</div>
* v. (cc5) The system SHALL capture identity of the user who entered/authored Record Entry content.
* vi. (cc6) The system SHALL capture identity of the system application which originated Record Entry content.
* vii. (cc7) IF the source of Record Entry content is a device, THEN the system SHALL capture identity of the device.
* viii. (cc8) The system SHALL capture the Action as evidenced by Record Entry content.
* ix. (cc9) The system SHALL capture the type of Record Event trigger (i.e., originate/retain).
* x. (cc10) The system SHALL capture the date and time of Action occurrence as evidenced by Record Entry content.
* <div id="publish-box">xi. (cc11) The system SHALL capture the date and time Record Entry content is originated.</div>
* xii. (cc12) The system MAY capture the duration of the Action evidenced by Record Entry content.
* xiii. (cc13) The system MAY capture the physical location of the Action evidenced by Record Entry content.
* xiv. (cc14) The system SHOULD capture identity of the location (i.e., network address) where Record Entry content is originated.
* xv. (cc15) The system MAY capture the rationale for the Action evidenced by Record Entry content.
* xvi. (cc16) The system MAY capture the rationale for originating Record Entry content.
* xvii. (cc17) IF Record Entry content includes templates (boilerplate information) or copied (duplicated) information, THEN the system SHOULD capture the source of such content.

**c. Amend Record Entry Content (Function RI.1.1.2)**
* i. (cc 1) The system SHALL provide the ability to update (amend) Record Entry content.
* ii. (cc2) The system SHALL maintain the original and all previously amended versions of the Record Entry, retaining each version instance without alteration.
* <div id="publish-box">iii. (cc3) The system SHALL capture a new uniquely identifiable version of the Record Entry, incorporating amended content.</div>
* iv. (cc4) The system SHALL capture the signature event (e.g., digital signature) of the amendment Author, binding signature to Record Entry content.

**d. Evidence of Record Entry Amendment Event (Function RI.1.1.2.1)**
* i. (cc1) The system SHALL audit each occurrence when a Record Entry is amended.
* ii. (cc2) The system SHALL capture identity of the organization where Record Entry content is amended.
* <div id="publish-box">iii. (cc3) The system SHALL capture identity of the patient who is subject of amended Record Entry content.</div>
* iv. (cc4) The system SHALL capture identity of the user who entered/authored Record Entry content amendment.
* v. (cc5) The system SHALL capture identity of the system application which amended Record Entry content.
* vi. (cc6) The system SHALL capture the type of Record Event trigger (i.e., amendment).
* <div id="publish-box">vii. (cc7) The system SHALL capture the date and time Record Entry content is amended.</div>
* viii. (cc8) The system SHOULD capture identity of the location (i.e., network address) where Record Entry content is amended.
* ix. (cc9) The system SHOULD capture the rationale for amending Record Entry content.
* x. (cc10) The system SHALL capture a sequence identifier for amended Record Entry content.
* xi. (cc11) The system SHOULD capture a reference (e.g., link, pointer) to pre-amendment data for each amended Record Entry.

**e. Receive and Retain Record Entries (Function RI.1.1.9)**
* i. (cc1) The system SHOULD provide the ability to capture and maintain Record Entry content from external systems, retaining and persisting original unaltered content and signature bindings, Action and Record Entry provenance and metadata.
* ii. (cc2) The system SHALL provide the ability to capture and maintain Record Entry extracts from external systems, retaining and persisting source, identity, record content, corresponding provenance and metadata.
* iii. (cc3) The system SHALL identify the patient or individual subject of received Record Entry content.
* iv. (cc4) IF received with Record Entry content, THEN the system SHOULD control subsequent data access to that permitted by corresponding authorizations and patient consents.

**f. Evidence of Receive/Retain Event (Function RI.1.1.9.1)**
* i. (cc1) The system SHALL audit each occurrence when externally-sourced Record Entry content is received and retained.
* ii. (cc2) The system SHALL capture identity of the organization transmitting Record Entry content received and retained.
* iii. (cc3) The system system SHALL capture identity of the organization receiving transmitted Record Entry content.
* iv. (cc4) The system SHALL capture identity of the patient who is subject of received Record Entry content
* v. (cc5) IF the system supports user verification of receipt of externally-sourced Record Entry content, THEN the system SHALL capture identity of the user accepting receipt of the transmitted Record Entry content.
* vi. (cc6) The system SHALL capture identity of the system application which transmitted Record Entry content.
* vii. (cc7) The system SHALL capture identity of the system application which received Record Entry content.
* viii. (cc8) The system SHALL capture the type of Record Event trigger (i.e., receive).
* ix. (cc9) The system SHALL capture the date and time Record Entry content is received.
* x. (cc10) The system SHOULD capture identity of the location (i.e., network address) where the Record Entry content is received.
* xi. (cc11) The system MAY capture the rationale for accepting receipt of transmitted Record Entry content.
* xii. (cc12) The system SHALL capture the type of Record Entry content received (e.g., original, amended, updated data).
* xiii. (cc13) IF an internal identifier is assigned to data/documents received from an external source, THEN the system MAY capture the data, document or other identifier for the Record Entry received.
* xiv. (cc14) The system MAY capture data elements for the Record Entry received.

---

{% include link-list.md %}
