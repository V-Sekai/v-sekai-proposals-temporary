# Distribute trusted clients with notary

## Context and Problem Statement

We use itch.io distribute our software clients.

1. Security concerns with trust. We do not control hosting.
1. Want ability to mirror package sources.
1. Research use to distribute avatars and worlds
1. Want something off the shelf

## Describe the proposed option and how it helps to overcome the problem or limitation

Use the notary system so we can establish trust.

### Describe how your proposal will work, with code, pseudo-code, mock-ups, and/or diagrams

We distribute the notary updater and make it fetch the launcher and V-Sekai.

We provide a notary server.

We setup the trust relationship during the install and maintance.

### Positive Consequences <!-- optional -->

- Code reviewed and trusted by large corporations (Docker Images) and in safety critial fields (Automobiles)
- Off the shelf

### Negative Consequences <!-- optional -->

- Unknown support costs

## Option graveyard Steam only

Steam provides a distribution network and marketplace.

List the reasons for the rejection: (the Bad traits)

* Third party trust

## Option graveyard Itch.io only

Itch.io provides a distribution network and marketplace.

List the reasons for the rejection: (the Bad traits)

* Third party trust

## If this enhancement will not be used often, can it be worked around with a few lines of script?

Not trivial. The documentaion of Notary start by the description of a possible security model and provides several attacks against it.

## Is there a reason why this should be core and done by us?

From a security standpoint, we need to ensure that there is a trust between the software we send and the client supply chain to get it.

## Links <!-- optional -->

- https://github.com/kolide/updater
- https://github.com/theupdateframework/notary
- https://github.com/theupdateframework/specification/blob/master/tuf-spec.md