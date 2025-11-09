# TravelledWaySection

A TravelledWaySection is a type of NetworkElement that represents an aggregation of TravelledWayLinks and TravelledWaySegments that jointly represent a contiguous length of a path that shares the same management and operational strategies (within the scope of interest of the implementation).

![TravelledWaySection Diagram](../diagrams/transportnetwork__TravelledWaySection.dot.svg)

<a href="../../diagrams/transportnetwork__TravelledWaySection.dot.svg">Open interactive TravelledWaySection diagram</a>

## Specializations of TravelledWaySection

| Class | Description |
|-------|-------------|
| [Footpath Section](transportnetwork__FootpathSection.md) | A FootpathSection is a type of TravelledWaySection that groups FootpathLinks and FootpathSegments for a useful operational purpose. |
| [Micromobility Path Section](transportnetwork__MicromobilityPathSection.md) | A MicromobilityPathSections is a type of RoadSection that groups MicromobilityLinks and MicromobilityPathSegments for a useful operational purpose (e.g., assigning a speed limit, designating areas of shared use). |
| [Rail Section](transportnetwork__RailSection.md) | A RailSection is a type of TravelledWaySection that groups TrackLinks and TrackSegments for a useful operational purpose (e.g., assigning a speed limit, designating a traffic control scheme). |
| [Road Section](transportnetwork__RoadSection.md) | A RoadSection is a type of TravelledWaySection that groups RoadLinks and RoadSegments for a useful operational purpose (e.g., assigning a speed limit, designating a traffic control scheme). |

## Formalization for TravelledWaySection

| Property | Constraint |
|----------|------------|
| partwhole::hasProperPart | all TravelledWayLink or TravelledWaySegment |
| partwhole::properPartOf | all TransportNetwork |
| partwhole::properPartOf | min 1 owl::Thing |
| subClassOf | NetworkElement |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TransportNetworkPattern |

