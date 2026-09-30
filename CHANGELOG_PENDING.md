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

#### General

#### Broadcaster

#### CLI
