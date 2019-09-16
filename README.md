# Jembi Openhim Docker Repository

The Dockerfiles for [Openhim](http://openhim.readthedocs.io/en/latest/) [Core](https://github.com/jembi/openhim-core-js) and [Console](https://github.com/jembi/openhim-console).

* Step 1: Add a new folder for new release candidate. The folder should have the same name as the release version, i.e. `1.0.0` for release `v1.0.0`

We use two branches to track the two sets of files:

* Step 3: Create a release tag. Name the tag as follows: {branch name}-{new release version}, i.e. `console-v1.0.0`

* Step 4: Log into docker hub to create a build setting for the new release. When adding a new build setting, use the following values:
  * Type: `Tag`
  * Name: {branch name}-{new release version}, i.e. `console-v1.0.0`
  * Dockerfile location: {Name of the newly created folder}
  * Docker Tag Name: release version, i.e. `1.0.0`
