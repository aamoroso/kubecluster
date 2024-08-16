# Overview
Spegel, mirror in Swedish, is a stateless cluster local OCI registry mirror.

Spegel is for you if you are looking to do any of the following:

- Locally cache images from external registries with no explicit configuration.
- Avoid cluster failure during external registry downtime.
- Improve image pull speed and pod startup time by pulling images from the local cache first.
- Avoid rate-limiting when pulling images from external registries (e.g. Docker Hub).
- Decrease egressing traffic outside of the clusters network.
- Increase image pull efficiency in edge node deployments.
