# TravelledWayLink

A TravelledWayLink is a type of NetworkElement and transinfras:TravelledWayLink. It represents a contiguous length of a TravelledWay between two TransportNodes of operational or managerial significance.

![TravelledWayLink Diagram](../diagrams/transportnetwork__TravelledWayLink.dot.svg)

<a href="../../diagrams/transportnetwork__TravelledWayLink.dot.svg">Open interactive TravelledWayLink diagram</a>

## Specializations of TravelledWayLink

| Class | Description |
|-------|-------------|
| [Footpath Link](transportnetwork__FootpathLink.md) | A Footpath Link is a type of TravelledWayLink designed for pedestrians. |
| [Micromobility Link](transportnetwork__MicromobilityLink.md) | A MicromobilityLink is a type of RoadLink designed for micromobility vehicles. |
| [Road Link](transportnetwork__RoadLink.md) | A RoadLink is a type of TravelledWayLink and transinfras:RoadLink using a stabilized base designed for the movement of vehicles that conform to a specified set of requirements but may be used by others as well. |
| [Track Link](transportnetwork__TrackLink.md) | A TrackLink is a type of TravelledWayLink that uses rails on a stabilized base. |
| [Travel Corridor Link](transportnetwork__TravelCorridorLink.md) | A TravelCorridorLink is a type of TravelledWayLink that is made up of TravelCorridorSegments. |

## Formalization for TravelledWayLink

| Property | Constraint |
|----------|------------|
| allowedDirections | all code::Code |
| allowedDirections | max 1 owl::Thing |
| from | all TransportNode |
| from | exactly 1 owl::Thing |
| partwhole::hasProperPart | all TravelledWaySegment |
| partwhole::properPartOf | all TransportNetwork or TravelledWay or TravelledWaySection |
| partwhole::properPartOf | min 1 owl::Thing |
| subClassOf | NetworkElement |
| subClassOf | transinfras::TravelledWayLink |
| to | all TransportNode |
| to | exactly 1 owl::Thing |

## Used by classes

| Class | Property |
|-------|----------|
| [Transport Node](transportnetwork__TransportNode.md) | egress |
| [Transport Node](transportnetwork__TransportNode.md) | ingress |
| [Travelled Way](transportnetwork__TravelledWay.md) | partwhole::hasProperPart |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TransportNetworkPattern |

