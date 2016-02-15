# Frugal event sourcing in Rust with Proust

## Short

Kafka reshaped the event sourcing ecosystem by providing a robust event log
system and proper foundations for an event sourced architecture with the Kappa
architecture.

Not every project operates at LinkedIn scale however, and running a kafka
cluster can be costly.  Proust was created as a single node, lightweight
alternative to kafka, while still using the kafka protocol. The
kafka-compatible tools work with proust, so it's still possible to spin up a
proper kafka cluster when the need arises.

To ensure optimal resource use on a single node, proust uses Rust.

The talk will present event sourcing architectures and their trade-offs, as
well as showcasing different uses and patterns in Rust used to write proust.

## Commentary

- Discover the bases of an event-sourced architecture
- Showcase uses of rust in the real world

## Target audience

People interested in using an event sourcing architecture, but who can't
afford to spin up a kafka cluster.
People curious about rust who want to
discover its uses in a practical setting.


