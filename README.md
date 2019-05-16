# Kublr CircleCi Orbs

The orbs are tested in .circleci/config.yaml of this repo.
Finished orbs will be published to the public CircleCi orb repository.

* Publish to dev first (before pushing changes to repo):
  * `circleci orb publish kublr-api/orb.yml kublr/kublr-api@dev:latest`

* Push orb changes to this repo to kick off tests for orb commands.

* Publish to production:
  * `circleci orb publish kublr-api/orb.yml kublr/kublr-api@<sem_ver>`

# Initial and one-time configuration

## Basic requirements

* GitHub project created and added to CircleCI app

* CircleCI API token created in CircleCI app and registered in `~/.circleci/cli.yml`
  * `circleci setup`

## Per CircleCI namespace

* CircleCI *kublr* namespace is registered
  * `circleci namespace create kublr github kublr`

## Per CircleCI orb

* CircleCI *kublr/kublr-api* orb is registered
  * `circleci orb create kublr/kublr-api`
