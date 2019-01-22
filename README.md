# Jembi Openhim Docker Repository

The Dockerfiles for [Openhim](http://openhim.readthedocs.io/en/latest/) [Core](https://github.com/jembi/openhim-core-js) and [Console](https://github.com/jembi/openhim-console).

<<<<<<< HEAD
These Dockerfiles are used to manage the docker images for releases of each Openhim repository.
=======
* Step 1: Add a new folder for new release candidate. The folder should have the same name as the release version, i.e. `1.0.0` for release `v1.0.0`
>>>>>>> f6461a8296b24b823181d61c08d1fe8a8a0c029a

We use two branches to track the two sets of files:

<<<<<<< HEAD
* [Core Dockerfiles](https://github.com/jembi/openhim-docker/tree/core)
* [Console Dockerfiles](https://github.com/jembi/openhim-docker/tree/console)
=======
* Step 3: Create a release tag. Name the tag as follows: {branch name}-{new release version}, i.e. `console-v1.0.0`

* Step 4: Log into docker hub to create a build setting for the new release. When adding a new build setting, use the following values:
  * Type: `Tag`
  * Name: {branch name}-{new release version}, i.e. `console-v1.0.0`
  * Dockerfile location: {Name of the newly created folder}
  * Docker Tag Name: release version, i.e. `1.0.0`
>>>>>>> f6461a8296b24b823181d61c08d1fe8a8a0c029a
