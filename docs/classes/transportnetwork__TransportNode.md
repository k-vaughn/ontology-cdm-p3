# TransportNode

A TransportNode is a NetworkElement that represents a node on the transport network that can be used to designate an end to a link or to join links.

![TransportNode Diagram](../diagrams/transportnetwork__TransportNode.dot.svg)

<a href="../../diagrams/transportnetwork__TransportNode.dot.svg">Open interactive TransportNode diagram</a>

## Specializations of TransportNode

| Class | Description |
|-------|-------------|
| [Junction](transportnetwork__Junction.md) | A Junction is a TransportNode that allows a traveller to connect from one TravelledWayLink to another. |
| [Route Point](transportnetwork__RoutePoint.md) | A RoutePoint represents a point of interest along a PublicTransportRoute. |

## Formalization for TransportNode

| Property | Constraint |
|----------|------------|
| egress | all TravelledWayLink |
| egress | min 1 owl::Thing |
| ingress | all TravelledWayLink |
| ingress | min 1 owl::Thing |
| partwhole::properPartOf | all TransportNetwork |
| partwhole::properPartOf | min 1 owl::Thing |
| subClassOf | NetworkElement |

## Used by classes

| Class | Property |
|-------|----------|
| [Travelled Way Link](transportnetwork__TravelledWayLink.md) | from |
| [Travelled Way Link](transportnetwork__TravelledWayLink.md) | to |

## Other annotations

| Annotation | Value |
|------------|-------|
| xsd::pattern | TransportNetworkPattern |

