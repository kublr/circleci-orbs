# Kublr CircleCi Orbs

The orbs are tested in .circleci/config.yaml of this repo.
Finished orbs will be published to the public CircleCi orb repository.

* Publish to dev first (before pushing changes to repo):
  * `circleci orb publish kublr-api/orb.yml kublr/kublr-api@dev:latest`

* Push orb changes to this repo to kick off tests for orb commands.

* Publish to production:
  * `circleci orb publish kublr-api/orb.yml kublr/kublr-api@<sem_ver>`
