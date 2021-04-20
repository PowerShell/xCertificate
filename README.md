# CertificateDsc

[![Build Status](https://dev.azure.com/dsccommunity/CertificateDsc/_apis/build/status/dsccommunity.CertificateDsc?branchName=main)](https://dev.azure.com/dsccommunity/CertificateDsc/_build/latest?definitionId=28&branchName=main)
![Code Coverage](https://img.shields.io/azure-devops/coverage/dsccommunity/CertificateDsc/28/main)
[![Azure DevOps tests](https://img.shields.io/azure-devops/tests/dsccommunity/CertificateDsc/28/main)](https://dsccommunity.visualstudio.com/CertificateDsc/_test/analytics?definitionId=28&contextType=build)
[![PowerShell Gallery (with prereleases)](https://img.shields.io/powershellgallery/vpre/CertificateDsc?label=CertificateDsc%20Preview)](https://www.powershellgallery.com/packages/CertificateDsc/)
[![PowerShell Gallery](https://img.shields.io/powershellgallery/v/CertificateDsc?label=CertificateDsc)](https://www.powershellgallery.com/packages/CertificateDsc/)
[![codecov](https://codecov.io/gh/dsccommunity/StorageDsc/branch/main/graph/badge.svg)](https://codecov.io/gh/dsccommunity/CertificateDsc)

## Code of Conduct

This project has adopted [this code of conduct](CODE_OF_CONDUCT.md).

## Releases

For each merge to the branch `main` a preview release will be
deployed to [PowerShell Gallery](https://www.powershellgallery.com/).
Periodically a release version tag will be pushed which will deploy a
full release to [PowerShell Gallery](https://www.powershellgallery.com/).

## Contributing

Please check out common DSC Community [contributing guidelines](https://dsccommunity.org/guidelines/contributing).

## Change log

A full list of changes in each version can be found in the [change log](CHANGELOG.md).

## Resources

The **CertificateDsc** module is a part of the Windows PowerShell Desired State
Configuration (DSC) Resource Kit, which is a collection of DSC Resources. This
module includes DSC resources that simplify administration of certificates on a
Windows Server, with simple declarative language.

The **CertificateDsc** module contains the following resources:

- **CertificateExport**: Used to export a certificate from a Windows certificate
  store.
- **CertificateImport**: Used to import a certificate into a Windows certificate
  store.
- **CertReq**: Used to request a new certificate from an certificate authority.
- **PfxImport**: Used to import a PFX certificate into a Windows certificate store.
- **WaitForCertificateServices**: Used to wait for a Active Directory Certificate
  Services Certificate Authority to become available.

This project has adopted [this code of conduct](CODE_OF_CONDUCT.md).

## Documentation and Examples

For a full list of resources in CertificateDsc and examples on their use, check out
the [CertificateDsc wiki](https://github.com/dsccommunity/CertificateDsc/wiki).

## Operating Systems

These resources are automatically tested on **Windows Server 2016** and
**Windows Server 2019**.

The resources should still work on Windows Server 2012 R2 and older operating
systems, but are will no longer be updated to work with these older versions.
The tests do not work on Windows Server 2012 R2 and older operating systems
because of the missing features in the `New-SelfSignedCertificate` function.
