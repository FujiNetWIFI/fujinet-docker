# fujinet-docker

A project to contain docker file definitions for various parts of fujinet that
can be built in docker containers.

## docker-compose.yml

Combines ATARI bridge and fujinet-pc.

This can be connected to via Altirra as normal.

### ports

- 9996/tcp is exposed for Altirra on the bridge
- 8000/tcp is exposed for FN WebUI in firmware


## Dockerfile.firmware

Builds fujinet-pc for ATARI. Future changes could make this a parameter to create different
versions for APPLE or COCO.

## Dockerfile.bridge

Runs the python bridge module for connecting Altirra to Fujinet-PC for Atari.
