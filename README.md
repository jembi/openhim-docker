# Jembi Openhim Docker Repository

Process for creating a new Openhim release on Docker hub.

* Step 1: Add a new folder for new release candidate. The folder should have the same name as the release version, i.e. `v1.0.0` for release `v1.0.0`

* Step 2: Copy the Dockerfile from one of the previous releases. Remember to change the version in Dockerfile to match the new release.

* Step 3: Create a release tag. Name the tag as follows: {new release version}, i.e. `v1.0.0`

* Step 4: Log into docker hub to create a build setting for the new release. When adding a new build setting, use the following values:
  * Type: `Tag`
  * Name: {new release version}, i.e. `v1.0.0`
  * Dockerfile location: Name of the newly created folder
  * Docker Tag Name: release version
