[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/aws-controllers-k8s/community/issues)
![GitHub issues](https://img.shields.io/github/issues-raw/aws-controllers-k8s/community?style=flat)
![GitHub](https://img.shields.io/github/license/aws-controllers-k8s/community?style=flat)
![GitHub watchers](https://img.shields.io/github/watchers/aws-controllers-k8s/community?style=social)
![GitHub stars](https://img.shields.io/github/stars/aws-controllers-k8s/community?style=social)
![GitHub forks](https://img.shields.io/github/forks/aws-controllers-k8s/community?style=social)

# AWS Controllers for Kubernetes (ACK)

**AWS Controllers for Kubernetes (ACK)** lets you define and use AWS service
resources directly from Kubernetes. With ACK, you can take advantage of AWS
managed services for your Kubernetes applications without needing to define
resources outside of the cluster or run services that provide supporting
capabilities like databases or message queues within the cluster.

ACK is an open source project built with ❤️  by AWS. The project is composed of
many source code repositories containing a [common runtime][runtime-repo], a
[code generator][codegen-repo] and Kubernetes custom controllers for individual
AWS service APIs.

[runtime-repo]: https://github.com/aws-controllers-k8s/runtime
[codegen-repo]: https://github.com/aws-controllers-k8s/code-generator

> **IMPORTANT** Please be sure to read our documentation about
> [release versioning and maintenance phases][releases] and note that ACK
> service controllers in the `Preview` maintenance phase are not recommended
> for production use. Use of ACK controllers in `Preview` maintenance phase is
> subject to the terms and conditions contained in the
> [AWS Service Terms][aws-service-terms], particularly the Beta Service
> Participation Service Terms, and apply to any service controllers in a
> `Preview` maintenance phase.

[releases]: https://aws-controllers-k8s.github.io/community/releases/
[aws-service-terms]: https://aws.amazon.com/service-terms

* [Overview](#overview)
* [Getting Started](#getting-started)
* [Help & Feedback](#help--feedback)
* [Contributing](#contributing)
* [License](#license)

## Overview

Kubernetes applications often require a number of supporting resources like
databases, message queues, and object stores. AWS provides a set of managed
services that you can use to provide these resources for your apps, but
provisioning and integrating them with Kubernetes was complex and time
consuming. ACK lets you define and consume AWS services and resources directly
from a Kubernetes cluster. It gives you a unified way to manage your
application and its dependencies.

ACK is a collection of Kubernetes [custom resource definitions][crd] (CRDs) and
custom controllers working together to extend the Kubernetes API and manage AWS
resources on your behalf.

[crd]: https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/

## Getting Started

Currently, there are a set of ACK [service controllers][services] that have
been released in a `Preview` [maintenance phase][maint-phases]. You may
[install][install] these controllers in binary form using the Helm charts
published on our ACK public artifact repository.

[services]: https://aws-controllers-k8s.github.io/community/services/
[maint-phases]: https://aws-controllers-k8s.github.io/community/releases#maintenance-phases
[install]: https://aws-controllers-k8s.github.io/user-docs/install/

If you are comfortable building Go code yourself and working with static
Kubernetes manifests, you are also free to [test-drive][testing] various
controllers using our KinD-based end-to-end test suite.

[testing]: https://aws-controllers-k8s.github.io/community/dev-docs/testing/

## Help & Feedback

For help, please consider the following venues (in order):

* [ACK project documentation](https://aws-controllers-k8s.github.io/community/)
* [Search open issues](https://github.com/aws-controllers-k8s/community/issues)
* [File an issue](https://github.com/aws-controllers-k8s/community/issues/new/choose)
* Chat with us on the `#provider-aws` channel in the [Kubernetes Slack](https://kubernetes.slack.com/) community.

## Contributing

We welcome community contributions and pull requests.

See our [contribution guide](/CONTRIBUTING.md) for more information on how to
report issues, set up a development environment, and submit code.

We adhere to the [Amazon Open Source Code of Conduct][coc].

You can also learn more about our [Governance](/GOVERNANCE.md) structure.

[coc]: https://aws.github.io/code-of-conduct

## License

This project is [licensed](/LICENSE) under the Apache-2.0 License.
