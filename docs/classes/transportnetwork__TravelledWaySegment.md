# TravelledWaySegment

A TravelledWaySegment is a type of a transinfras:TravelledWaySegment and NetworkElement that represents a contiguous length of a TravelledWayLink characterized by the same physical characteristics.

![TravelledWaySegment Diagram](../diagrams/transportnetwork__TravelledWaySegment.dot.svg)

<a href="../../diagrams/transportnetwork__TravelledWaySegment.dot.svg">Open interactive TravelledWaySegment diagram</a>

## Specializations of TravelledWaySegment

| Class | Description |
|-------|-------------|
| [Footpath Segment](transportnetwork__FootpathSegment.md) | A FootpathSegment is a type of TravelledWaySegment that represents a portion of a FootpathLink with common physical characteristics. |
| [Micromobility Path Segment](transportnetwork__MicromobilityPathSegment.md) | A MicromobilityPathSegment is a type of RoadSegment that represents a portion of a MicromobilityLink with common physical characteristics. |
| [Road Segment](transportnetwork__RoadSegment.md) | A RoadSegment is a type of TravelledWaySegment and transinfas:RoadSegment that represents a portion of a RoadLink with common physical characteristics. |
| [Track Segment](transportnetwork__TrackSegment.md) | A TrackSegment is a type of TravelledWaySegment that represents a portion of a TrackLink with common physical characteristics. |
| [Travel Corridor Segment](transportnetwork__TravelCorridorSegment.md) | A TravelCorridorSegment is a type of TravelledWaySegment that logically groups multiple TravelledWaySegments together as being co-located or side-by-side. |

## Formalization for TravelledWaySegment

| Property | Constraint |
|----------|------------|
| partwhole::hasProperPart | all TravelledWayLane |
| partwhole::hasProperPart | min 1 owl::Thing |
| partwhole::properPartOf | all TravelledWayLink or TravelledWaySection |
| partwhole::properPartOf | min 1 owl::Thing |
| subClassOf | NetworkElement |
| subClassOf | transinfras::TravelledWaySegment |
| travelCorridorSegment | all TravelCorridorSegment |

## Used by classes

| Class | Property |
|-------|----------|
| [Travel Corridor Segment](transportnetwork__TravelCorridorSegment.md) | corridorElement |
| [Travelled Way Lane](transportnetwork__TravelledWayLane.md) | partwhole::properPartOf |
| [Travelled Way Link](transportnetwork__TravelledWayLink.md) | partwhole::hasProperPart |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TransportNetworkPattern |

