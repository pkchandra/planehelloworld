# Changelog
All notable changes to chart **helloworld-go** are documented in this file,
which is effectively a **Release Note** and readable by customers.

Do take a minute to read how to format this file properly.
It is based on [Keep a Changelog](http://keepachangelog.com)
- Newer entries _above_ older entries.
- At minimum, every released (stable) version must have an entry.
- Pre-release or incubating versions may reuse `Unreleased` section.

## [1.3.51] - 2024-02-12
### Fixed
- security context setting

## [1.3.50] - 2024-02-08
### Fixed
- Container security context configuration (CSFS-57501)

## [1.3.49] - 2024-01-16
### Added
- Add readOnlyRootFileSystem:true and allowPrivilegeEscalation:false to other jobs

## [1.3.48] - 2023-10-25
### Added
- Add readOnlyRootFileSystem:true and allowPrivilegeEscalation:false to hooks

## [1.3.47] - 2023-06-04
### Added
- Hooks can be configured to fail-on-demand (configuration read from ConfigMap).
## [1.3.46] - 2023-01-11
### Added
- Add readOnlyRootFileSystem:true and allowPrivilegeEscalation:false for jobs
- Add securityContext for jobs

## [1.3.45] - 2023-01-05
### Added
- Add resources for heal/scale hooks

## [1.3.44] - 2022-11-28
### Changed
- Cbur brpolicy auto detection

## [1.3.43] - 2022-11-08
### Changed
- Updated helloworld_go image to 1.0.7

## [1.3.42] - 2022-09-19
### Added
- Support for multiple hook jobs

## [1.3.41] - 2022-08-29
### Changed
- Updated helloworld_go image to 1.0.6

## [1.3.40] - 2022-07-29
### Changed
- Changed deprecated registry FQDN

## [1.3.39] - 2022-06-30
### Changed
- Added resource quota for jobs

## [1.3.38] - 2022-05-24
### Changed
- Ingress format v1

## [1.3.37] - 2021-12-21
### Fixed
- update securityContext configuration
- rbac enabled flag according to HBP

## [1.3.36] - 2021-12-20
### Fixed
- update cpu requests to 50m

## [1.3.35] - 2021-11-25
### Fixed
- add readOnlyRootFileSystem:true and allowPrivilegeEscalation:false

## [1.3.34] - 2021-08-18
### Fixed
- hook template

## [1.3.33] - 2021-07-12
### Fixed
- type in 1.3.32 for hook
## [1.3.32] - 2021-07-09
### Changed
- factory resources and securityContext in values
- reduce request resources

## [1.3.31] - 2021-02-22
### Changed
- fix helloworld-go test

## [1.3.30] - 2020-11-30
### Changed
- fix hooks for helm heal test

## [1.3.29] - 2020-11-25
### Changed
- add hooks for helm plugin test

## [1.3.28] - 2020-10-22
### Changed
- fix latest tag for images

## [1.3.27] - 2020-10-13
### Changed
- fix hook weight for post-delete job

## [1.3.26] - 2020-09-28
### Changed
- helloworld image reads language from env variable 

## [1.3.25] - 2020-09-16 
### Changed
- helloworld image version

## [1.3.24] - 2020-08-27
### Changed
- change to static pvc name
- add post-delete hook to check deleted pvc

## [1.3.23] - 2020-08-13
### Changed
- duplicate 1.3.22 for ncm tests uses

## [1.3.22] - 2020-08-13
### Changed
- decrease resuested ressources( memory& cpu)

## [1.3.21] - 2020-07-07
### Changed
- add apiVersion logic to support legacy k8s version on deployment

## [1.3.20] - 2020-06-30
### Changed
- Change the ingress apiVersion


## [1.3.19] - 2020-05-19
### Changed
- Change the description 

## [1.3.16] - 2020-05-15
### Added
- add the path for ingress

## [1.3.15] - 2020-05-12
### Changed
- fix the tls configuration

## [1.3.14] - 2020-05-11
### Added
- add tls configuration 

## [1.3.13] - 2020-04-16
### Changed
- fix rbac issue - CSFS-23327 

## [1.3.12] - 2020-04-15
### Changed
- fix pre delete job


## [1.3.11] - 2020-04-15
### Added
- add test for deleting a chart that has a dependency 

  
## [1.3.10] - 2020-03-03
### Changed
- fixed helm3 compliant
  
## [1.3.9] - 2020-01-30
### Changed
- fixed hooks for undeleted jobs

## [1.3.8] - 2019-11-14
### Changed
- fixed cbur bug and updated k8s version

## [1.3.7] - 2019-11-4
### Changed
- add hook sleep in cases: pre/post | install/update/delete

## [1.3.6] - 2019-10-31
### Changed
- add quota

## [1.3.5] - 2019-10-24
### Changed
- add pre-install hook

## [1.3.4] - 2019-10-15
### Changed
- storageclass condition


## [1.3.3] - 2019-09-02
### Changed
- replica set to 1
- storageclass name and storage demanded 


## [1.3.2] - 2019-08-20
### Added
- k8s_wait test for job
- clusterrolebinding file

## [1.3.1] - 2019-07-17
### Fixed
- template storageclassname 

## [1.3.0] - 2019-07-16
### Fixed
- use derivepassword for pvc unique names
- changes image.replica to replicas


## [1.2.9] - 2019-07-01
### Fixed
- pvc with random name

## [1.2.8] - 2019-05-23
### Fixed
- brpolicy and deployment files
### Added
- pvc file

## [1.2.7] - 2019-05-17
### Fixed
- no chart change, pipeline replaces upload with csf-jenkinslib csfArtifactsPublish

## [1.2.6] - 2019-03-09
### Fixed
- no chart change, validiate chart promotion incubator to stable

## [1.2.5] - 2019-03-09
### Fixed
- no chart change, validiate chart promotion incubator to stable

## [1.2.4] - 2019-03-07
### Fixed
- validating chart promotion

## [1.2.3] - 2018-11-14
### Added
- helm test example

## [1.2.2] - 2018-11-09
### Added
- BrPolicy file 
### Added
- CSF chart relocation rules enforced

## [1.2.1] - 2018-08-14
### Added
- All future chart versions shall provide a change log summary

## [0.0.0] - YYYY-MM-DD
### Added | Changed | Deprecated | Removed | Fixed | Security
- your change summary, this is not a **git log**!

