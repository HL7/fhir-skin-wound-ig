---
title: Profiles and Extensions
layout: default
active: profiles
---
## Profiles and Extensions (Hierarchy)

* **Condition** [WoundAssert](StructureDefinition-WoundAssert.html)
  * _Extension_ [PresentOnAdmissionExt](StructureDefinition-PresentOnAdmissionExt.html)
  * _Extension_ [PressureUlcerAssociationExt](StructureDefinition-PressureUlcerAssociationExt.html)
  * _Extension_ [WoundAssessmentInterpretationExt](StructureDefinition-WoundAssessmentInterpretationExt.html)
  * _Extension_ [EpisodeExt](StructureDefinition-EpisodeExt.html)
  * _Extension_ [TrendExt](StructureDefinition-TrendExt.html)
  * _Extension_ [PeriwoundConditionExt](StructureDefinition-PeriwoundConditionExt.html)
  * _Extension_ [WoundTypeEtiologyExt](StructureDefinition-WoundTypeEtiologyExt.html)
  * _Extension_ [WoundImageExtension](StructureDefinition-WoundImageExtension.html)
  * _Extension_ [WoundInternalItemOrBodyStructureVisibleExt](StructureDefinition-WoundInternalItemOrBodyStructureVisibleExt.html)
  * _Extension_ [WoundGradationExt](StructureDefinition-WoundGradationExt.html)
  * _Extension_ [WoundRelatedObservationsPanelExt](StructureDefinition-WoundRelatedObservationsPanelExt.html)
    * **Observation** [WoundRelatedObservationsPanel](StructureDefinition-WoundRelatedObservationsPanel.html)
  * _Extension_ [BodyLocationExt](StructureDefinition-BodyLocationExt.html)
    * _Extension_ [AnatomicLocationExt](StructureDefinition-AnatomicLocationExt.html)
    * _Extension_ [BodySideExt](StructureDefinition-BodySideExt.html)
    * _Extension_ [BodyLocationOrientationExt](StructureDefinition-BodyLocationOrientationExt.html)
    * _Extension_ [UnderlyingAnatomicalStructureExt](StructureDefinition-UnderlyingAnatomicalStructureExt.html)
    * _Extension_ [BodyLandmarkOrientationExt](StructureDefinition-BodyLandmarkOrientationExt.html)
      * _Extension_ [BodyLandmarkDescriptionExt](StructureDefinition-BodyLandmarkDescriptionExt.html)
      * _Extension_ [ClockFacePositionExt](StructureDefinition-ClockFacePositionExt.html)
      * _Extension_ [DistanceFromLandmarkExt](StructureDefinition-DistanceFromLandmarkExt.html)
        * _Extension_ [DeviceExt](StructureDefinition-DeviceExt.html)
        * _Extension_ [DistanceFromLandmarkMeasurementExt](StructureDefinition-DistanceFromLandmarkMeasurementExt.html)
      * _Extension_ [SurfaceOrientationExt](StructureDefinition-SurfaceOrientationExt.html)
    * _Extension_ [BodyLocationQualifierExt](StructureDefinition-BodyLocationQualifierExt.html)
  * _Extension_ [WoundRecurrenceExt](StructureDefinition-WoundRecurrenceExt.html)
    * _Extension_ [PeriodicityExt](StructureDefinition-PeriodicityExt.html)
    * _Extension_ [RecurrenceExt](StructureDefinition-RecurrenceExt.html)


* **Observation** [WoundRelatedObservationsPanel](StructureDefinition-WoundRelatedObservationsPanel.html)
  * _Extension_ [WoundTunnelingAssertExt](StructureDefinition-WoundTunnelingAssertExt.html)
    * **Condition** [WoundTunnelingAssert](StructureDefinition-WoundTunnelingAssert.html)
  * _Extension_ [WoundUnderminingAssertExt](StructureDefinition-WoundUnderminingAssertExt.html)
    * **Condition** [WoundUnderminingAssert](StructureDefinition-WoundUnderminingAssert.html)
  * _Extension_ [WoundExudateAssertExt](StructureDefinition-WoundExudateAssertExt.html)
    * **Condition** [WoundExudateAssert](StructureDefinition-WoundExudateAssert.html)
  * **Observation** _hasMember_ [WoundBed](StructureDefinition-WoundBed.html)
  * **Observation** _hasMember_ [WoundEdge](StructureDefinition-WoundEdge.html)
  * **Observation** _hasMember_ [WoundSize](StructureDefinition-WoundSize.html)
  * **Observation** _hasMember_ [WoundShape](StructureDefinition-WoundShape.html)


* **Condition** [WoundTunnelingAssert](StructureDefinition-WoundTunnelingAssert.html)
  * _Extension_ [WoundTunnelingDirectionExt](StructureDefinition-WoundTunnelingDirectionExt.html)
    * **Observation** [WoundTunnelingDirection](StructureDefinition-WoundTunnelingDirection.html)
  * _Extension_ [WoundTunnelingLengthExt](StructureDefinition-WoundTunnelingLengthExt.html)
    * **Observation** [WoundTunnelingLength](StructureDefinition-WoundTunnelingLength.html)


* **Condition** [WoundUnderminingAssert](StructureDefinition-WoundUnderminingAssert.html)
  * _Extension_ [WoundUnderminingDirectionExt](StructureDefinition-WoundUnderminingDirectionExt.html)
    * **Observation** [WoundUnderminingDirection](StructureDefinition-WoundUnderminingDirection.html)
  * _Extension_ [WoundUnderminingLengthExt](StructureDefinition-WoundUnderminingLengthExt.html)
    * **Observation** [WoundUnderminingLength](StructureDefinition-WoundUnderminingLength.html)


* **Condition** [WoundExudateAssert](StructureDefinition-WoundExudateAssert.html)
  * _Extension_ [WoundExudateAppearanceExt](StructureDefinition-WoundExudateAppearanceExt.html)
    * **Observation** [WoundExudateAppearance](StructureDefinition-WoundExudateAppearance.html)
  * _Extension_ [WoundExudateColorExt](StructureDefinition-WoundExudateColorExt.html)
    * **Observation** [WoundExudateColor](StructureDefinition-WoundExudateColor.html)
  * _Extension_ [WoundExudateOdorExt](StructureDefinition-WoundExudateOdorExt.html)
    * **Observation** [WoundExudateOdor](StructureDefinition-WoundExudateOdor.html)
  * _Extension_ [WoundExudateVolumeExt](StructureDefinition-WoundExudateVolumeExt.html)
    * **Observation** [WoundExudateVolume](StructureDefinition-WoundExudateVolume.html)
  * _Extension_ [WoundExudateAmountDescriptionExt](StructureDefinition-WoundExudateAmountDescriptionExt.html)
    * **Observation** [WoundExudateAmountDescription](StructureDefinition-WoundExudateAmountDescription.html)


* **Observation** [WoundBed](StructureDefinition-WoundBed.html)
  * **Observation** _hasMember_ [WoundBedAppearance](StructureDefinition-WoundBedAppearance.html)
  * **Observation** _hasMember_ [WoundBedColor](StructureDefinition-WoundBedColor.html)


* **Observation** [WoundEdge](StructureDefinition-WoundEdge.html)
  * **Observation** _hasMember_ [WoundEdgeColor](StructureDefinition-WoundEdgeColor.html)
  * **Observation** _hasMember_ [WoundEdgeDescription](StructureDefinition-WoundEdgeDescription.html)


* **Observation** [WoundSize](StructureDefinition-WoundSize.html)
  * _Extension_ [DeviceExt](StructureDefinition-DeviceExt.html)


* **Observation** [WoundExudateVolume](StructureDefinition-WoundExudateVolume.html)
  * _Extension_ [EstimatedIndExt](StructureDefinition-EstimatedIndExt.html)

<br />

## Profiles (A-Z)

The following Profiles and have been defined for this implementation guide.

|Resource Type|Profile Name|
|---|---|
|Condition|[WoundAssert](StructureDefinition-WoundAssert.html)|
|Condition|[WoundExudateAssert](StructureDefinition-WoundExudateAssert.html)|
|Condition|[WoundTunnelingAssert](StructureDefinition-WoundTunnelingAssert.html)|
|Condition|[WoundUnderminingAssert](StructureDefinition-WoundUnderminingAssert.html)|
|Observation|[WoundBedAppearance](StructureDefinition-WoundBedAppearance.html)|
|Observation|[WoundBedColor](StructureDefinition-WoundBedColor.html)|
|Observation|[WoundBed](StructureDefinition-WoundBed.html)|
|Observation|[WoundEdgeColor](StructureDefinition-WoundEdgeColor.html)|
|Observation|[WoundEdgeDescription](StructureDefinition-WoundEdgeDescription.html)|
|Observation|[WoundEdge](StructureDefinition-WoundEdge.html)|
|Observation|[WoundExudateAmountDescription](StructureDefinition-WoundExudateAmountDescription.html)|
|Observation|[WoundExudateAppearance](StructureDefinition-WoundExudateAppearance.html)|
|Observation|[WoundExudateColor](StructureDefinition-WoundExudateColor.html)|
|Observation|[WoundExudateOdor](StructureDefinition-WoundExudateOdor.html)|
|Observation|[WoundExudateVolume](StructureDefinition-WoundExudateVolume.html)|
|Observation|[WoundRelatedObservationsPanel](StructureDefinition-WoundRelatedObservationsPanel.html)|
|Observation|[WoundShape](StructureDefinition-WoundShape.html)|
|Observation|[WoundSize](StructureDefinition-WoundSize.html)|
|Observation|[WoundTunnelingDirection](StructureDefinition-WoundTunnelingDirection.html)|
|Observation|[WoundTunnelingLength](StructureDefinition-WoundTunnelingLength.html)|
|Observation|[WoundUnderminingDirection](StructureDefinition-WoundUnderminingDirection.html)|
|Observation|[WoundUnderminingLength](StructureDefinition-WoundUnderminingLength.html)|

<!-- Uncomment for default generated list
include list-simple-structuredefinitions.xhtml
-->

<br />

## Extensions (A-Z)

The following [Extensions]({{site.data.fhir.path}}extensibility.html) have been defined as part of the Lower Extremity Skin Wound Assessment implementation Guide. A [registry of standard extensions]({{site.data.fhir.path}}extensibility-registry.html) can be found in the FHIR specification and additional extensions may be registered on the HL7 FHIR registry at http://hl7.org/fhir/registry.

|Extension Name
|---|
|[AnatomicLocationExt](StructureDefinition-AnatomicLocationExt.html)|
|[BodyLandmarkDescriptionExt](StructureDefinition-BodyLandmarkDescriptionExt.html)|
|[BodyLandmarkOrientationExt](StructureDefinition-BodyLandmarkOrientationExt.html)|
|[BodyLocationExt](StructureDefinition-BodyLocationExt.html)|
|[BodyLocationOrientationExt](StructureDefinition-BodyLocationOrientationExt.html)|
|[BodyLocationQualifierExt](StructureDefinition-BodyLocationQualifierExt.html)|
|[BodySideExt](StructureDefinition-BodySideExt.html)|
|[ClockFacePositionExt](StructureDefinition-ClockFacePositionExt.html)|
|[DeviceExt](StructureDefinition-DeviceExt.html)|
|[DistanceFromLandmarkExt](StructureDefinition-DistanceFromLandmarkExt.html)|
|[DistanceFromLandmarkMeasurementExt](StructureDefinition-DistanceFromLandmarkMeasurementExt.html)|
|[EpisodeExt](StructureDefinition-EpisodeExt.html)|
|[PeriwoundConditionExt](StructureDefinition-PeriwoundConditionExt.html)|
|[PresentOnAdmissionExt](StructureDefinition-PresentOnAdmissionExt.html)|
|[PressureUlcerAssociationExt](StructureDefinition-PressureUlcerAssociationExt.html)|
|[RecurrenceExt](StructureDefinition-RecurrenceExt.html)|
|[SurfaceOrientationExt](StructureDefinition-SurfaceOrientationExt.html)|
|[TrendExt](StructureDefinition-TrendExt.html)|
|[UnderlyingAnatomicalStructureExt](StructureDefinition-UnderlyingAnatomicalStructureExt.html)|
|[WoundAssessmentInterpretationExt](StructureDefinition-WoundAssessmentInterpretationExt.html)|
|[WoundExudateAmountDescriptionExt](StructureDefinition-WoundExudateAmountDescriptionExt.html)|
|[WoundExudateAppearanceExt](StructureDefinition-WoundExudateAppearanceExt.html)|
|[WoundExudateAssertExt](StructureDefinition-WoundExudateAssertExt.html)|
|[WoundExudateColorExt](StructureDefinition-WoundExudateColorExt.html)|
|[WoundExudateOdorExt](StructureDefinition-WoundExudateOdorExt.html)|
|[WoundExudateVolumeExt](StructureDefinition-WoundExudateVolumeExt.html)|
|[WoundGradationExt](StructureDefinition-WoundGradationExt.html)|
|[WoundImageExtension](StructureDefinition-WoundImageExtension.html)|
|[WoundInternalItemOrBodyStructureVisibleExt](StructureDefinition-WoundInternalItemOrBodyStructureVisibleExt.html)|
|[WoundRecurrenceExt](StructureDefinition-WoundRecurrenceExt.html)|
|[WoundRelatedObservationsPanelExt](StructureDefinition-WoundRelatedObservationsPanelExt.html)|
|[WoundTunnelingAssertExt](StructureDefinition-WoundTunnelingAssertExt.html)|
|[WoundTunnelingDirectionExt](StructureDefinition-WoundTunnelingDirectionExt.html)|
|[WoundTunnelingLengthExt](StructureDefinition-WoundTunnelingLengthExt.html)|
|[WoundTypeEtiologyExt](StructureDefinition-WoundTypeEtiologyExt.html)|
|[WoundUnderminingAssertExt](StructureDefinition-WoundUnderminingAssertExt.html)|
|[WoundUnderminingDirectionExt](StructureDefinition-WoundUnderminingDirectionExt.html)|
|[WoundUnderminingLengthExt](StructureDefinition-WoundUnderminingLengthExt.html)|

<!-- Uncomment for default generated list
include list-simple-extensions.xhtml
-->

{% include link-list.md %}

<br />


