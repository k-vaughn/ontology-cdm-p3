# TravelCorridorSegment

A TravelCorridorSegment is a type of TravelledWaySegment that logically groups multiple TravelledWaySegments together as being co-located or side-by-side.

![TravelCorridorSegment Diagram](../diagrams/transportnetwork__TravelCorridorSegment.dot.svg)

<a href="../../diagrams/transportnetwork__TravelCorridorSegment.dot.svg">Open interactive TravelCorridorSegment diagram</a>

## Formalization for TravelCorridorSegment

| Property | Constraint |
|----------|------------|
| corridorElement | all TravelledWaySegment |
| corridorElement | min 1 owl::Thing |
| partwhole::properPartOf | all TravelCorridorLink |
| subClassOf | TravelledWaySegment |

## Used by classes

| Class | Property |
|-------|----------|
| [Travel Corridor Link](transportnetwork__TravelCorridorLink.md) | partwhole::hasProperPart |
| [Travelled Way Segment](transportnetwork__TravelledWaySegment.md) | travelCorridorSegment |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TravelCorridorPattern |

