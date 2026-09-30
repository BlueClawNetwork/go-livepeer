# Unreleased Changes

## v0.X.X

### Breaking Changes 🚨🚨

### Features ⚒

#### General

- Remote signer: leave evidence when a `create_signed_ticket` event is dropped (`livepeer_remote_signer_events_dropped_total` counter, an error log with the ids needed to reconstruct the record) and expose `livepeer_remote_signer_event_queue_length`. Add `-kafkaRequireDelivery` and `-kafkaEnqueueTimeout` to refuse signing when the event cannot be enqueued.

#### Broadcaster

#### Orchestrator

#### Transcoder

### Bug Fixes 🐞

- Remote signer: `-remoteDiscovery` fetched each orchestrator's `/discovery` with a verifying HTTP client and failed against the self-signed certificate every orchestrator serves, while the gRPC call to the same node succeeded; the fetch now skips verification like the rest of the node's orchestrator calls.

#### General

#### Broadcaster

#### CLI
