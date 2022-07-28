# Extensibility options for Online Validation Service
[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/s4hana-online-validation-extension)](https://api.reuse.software/info/github.com/SAP-samples/s4hana-online-validation-extension)

## Description
<!-- Please include SEO-friendly description, SEO = improve rating for search engines -->
You use the [Online Validation](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/b2d44c1091094b5a810c2a879ee95522/79560d16dcc94299992ae4434d8694aa.html?version=2021.001) to verify selected system data (for example, master data held for a business partner) with an external service (for example, an online service or statutory database).
You would like to extend the Online Validation functions with validation with another external service.

## Requirements
The extensibility options are available in all SAP NetWeaver-based product with SAP_BASIS 75C and newer. This means that among others, all S/4 HANA releases are supported. 
It is necessary to implement all SAP Notes referred in the SAP Note [3085468](https://launchpad.support.sap.com/#/notes/3085468) or upgrade to the respective Support Package levels. 
The information in this repository is intended for ABAP Developers. 

## Download and Installation
This repository contains a step-by-step guide how to develop an own validation including an example class that can be used as a base for your development. You can [clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) the repository to your computer or import the repository to your ABAP system using e.g. [abapGit](https://docs.abapgit.org/).

## Implementation
The step-by-step implementation of an own validation is described [here](doc/ProcessDescription.md). 

## Known Issues
No known issues. 

## How to obtain support
[Create an issue](https://github.com/SAP-samples/s4hana-online-validation-extension/issues) in this repository if you find a bug or have questions about the content.
 
For additional support, [ask a question in SAP Community](https://answers.sap.com/questions/ask.html).

## Contributing
If you wish to contribute code, offer fixes or improvements, please send a pull request. Due to legal reasons, contributors will be asked to accept a DCO when they create the first pull request to this project. This happens in an automated fashion during the submission process. SAP uses [the standard DCO text of the Linux Foundation](https://developercertificate.org/).

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSE) file.

## Useful links
- [Download or Clone a GitHub repository](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
- [MD language Cheat sheet](https://www.markdownguide.org/cheat-sheet/)

## Updates:
| Date | Author | Description | 
| ------------ | ----------- | --------------------------------------------------- |
| July 28, 2022 | I334850 | Initial commit. |

