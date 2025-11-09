# FootpathLane

A FootpathLane is a type of TravelledWayLane that forms part of a FootpathSegment.

![FootpathLane Diagram](../diagrams/transportnetwork__FootpathLane.dot.svg)

<a href="../../diagrams/transportnetwork__FootpathLane.dot.svg">Open interactive FootpathLane diagram</a>

## Formalization for FootpathLane

| Property | Constraint |
|----------|------------|
| partwhole::properPartOf | all FootpathSegment |
| partwhole::properPartOf | min 1 owl::Thing |
| subClassOf | TravelledWayLane |

## Used by classes

| Class | Property |
|-------|----------|
| [Footpath Segment](transportnetwork__FootpathSegment.md) | partwhole::hasProperPart |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | PedestrianNetworkPattern |

