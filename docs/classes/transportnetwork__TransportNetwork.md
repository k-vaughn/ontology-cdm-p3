# TransportNetwork

A TransportNetwork is a NetworkElement that is a collection of other network elements that jointly represent a network of paths along which entities (e.g., vehicles, pedestrians) of a specified mode can operate.

![TransportNetwork Diagram](../diagrams/transportnetwork__TransportNetwork.dot.svg)

<a href="../../diagrams/transportnetwork__TransportNetwork.dot.svg">Open interactive TransportNetwork diagram</a>

## Specializations of TransportNetwork

| Class | Description |
|-------|-------------|
| [Footpath Network](transportnetwork__FootpathNetwork.md) | A FootpathNetwork is a type of TransportNetwork designed for the use of pedestrians but may be used by others as well. |
| [Micromobility Network](transportnetwork__MicromobilityNetwork.md) | A MicromobilityNetwork is a type of RoadNetwork designed for the use of micromobility vehicles, which have more limited performance characteristics than motor vehicles. |
| [Rail Network](transportnetwork__RailNetwork.md) | A RailNetwork is a type of TransportNetwork using rails on a stabilized base. |
| [Road Network](transportnetwork__RoadNetwork.md) | A RoadNetwork is a type of TransportNetwork using a stabilized base designed for the movement of vehicles, other than rail or air vehicles, that conform to a specified set of requirements but may be used by others as well. |

## Formalization for TransportNetwork

| Property | Constraint |
|----------|------------|
| partwhole::hasProperPart | all TransportNetwork or TransportNode or TravelledWay or TravelledWayLink or TravelledWaySection |
| partwhole::properPartOf | all TransportNetwork |
| subClassOf | NetworkElement |

## Used by classes

| Class | Property |
|-------|----------|
| [Transport Network](transportnetwork__TransportNetwork.md) | partwhole::properPartOf |
| [Transport Node](transportnetwork__TransportNode.md) | partwhole::properPartOf |
| [Travelled Way](transportnetwork__TravelledWay.md) | partwhole::properPartOf |
| [Travelled Way Section](transportnetwork__TravelledWaySection.md) | partwhole::properPartOf |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TransportNetworkPattern |

