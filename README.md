<div align="center">
	<img src="https://www.dropbox.com/s/b0xr4dgjk0g274y/hurtle-logo.png?dl=1" alt="Watchtower" title="Watchtower">
	<img src="https://www.dropbox.com/s/5snsos1ioryyern/hurtle-logo-text.png?dl=1" alt="Watchtower" title="Watchtower">
</div>

# Hurtle?
```
Q: Why is it called Hurtle?
A: Cos we like turtles

Q: What is your motto?
A: "Confusing name, simple orchestration"
```

# Why Hurtle?

hurtle lets you:

> offer your software as a service i.e. hurtle-it

This is the key aim of hurtle. Hurtle can take almost any software and offer it as a service to end-users. Its functionality all revolves around this idea, so the service offered is also one that can be designed with the cloud in mind, based on the [cloud-native application research of the ICCLab]().

## Where from?
Hurtle's origin is in the telcom world and in particular Network Function Virtualisation. Here hurtle has been used to offer services that have been to date ran directly on or embedded in hardware.

# Overview

Hurtle  is an open-source cloud service orchestrator. Hurtle is proven: it is the software that orchestrates the [Mobile Cloud Networking Project](http://www.mobile-cloud-networking.eu/site/).

This repository provides documentation for the overall Hurtle project and
pointers to the other repositories that make up a complete Hurtle deployment.
See the [repository list](./docs/developer-guide/repos.md).

Report bugs and request features using [GitHub Issues](https://github.com/icclab/hurtle/issues). For additional resources, you can contact the maintainers directly.

Hurtle consists of the following components:

- component 1
- component 2
- component 3

For more details, see:

- [Hurtle Architecture](./docs/architecture.md) for
  overall architecture.
- [Hurtle Reference](./docs/reference.md) for an
  overview of each component.
- The [herp derp](./docs/developer-guide/herpderp.md) for herp derp

# Features

 - Complete orchestration of your software
   - Resources it uses (e.g. virtual machines, networks)
   - External services it needs
 - Multi-dc/multi-region support
   - including inter-DC connectivity
 - Easy implementation of your service API
 - Guided implementation of your service instance manager
   - Many languages supported including Python, Java, Perl, PHP
   - Demo applications available
 - Scalable runtime management
 - Complete end-to-end logging of your software
 - Integration with [OpenStack](), [ICCLab's Joyent SDC contribs]()
 - Handle potential incidents of your software
   - Integration with [ICCLab's Watchtower (Cloud Incident Management)](https://github.com/icclab/watchtower-common)
 - Bill for your software and services
   - Integration with [ICCLab's Cyclops (Rating, charging & Billing)](https://icclab.github.io/cyclops/)
 - Leverages Open Cloud Standards (OCCI, OpenStack)


# Roadmap
Hurtling along soon:

 - Enhanced workload placement, dynamic policy-based
 - Support for docker-registry deployed containers
 - Runtime updates to service and resource topologies
 - CI and CD support
   - safe monitored dynamic service updates
 - TOSCA support
 - Support for VMware and CloudStack
 - User interface to visualise resource and services relationships
 - Additional external service endpoint protocol support


## Community

Community discussion about SmartDataCenter happens in one main place:

* The *hurtle-discuss* mailing list. Once you [subscribe to the list](#TODO: LINK),
  you can send mail to the list address: #TODO: adress.
  The mailing list archives are also [available on the web](#TODO: LINK).


You can also follow [@hurtle_orch](https://twitter.com/hurtle_orch) on
Twitter for updates.


## Getting Started
### Developer setup with devstack

1. ```curl https://get.hurtle.io | bash```
2. ???
3. Profit

### Installing Hurtle on OpenStack

Please see the [installation guide](./docs/installation_guide.md) for more details.

## Building

Good Luck...

## Contributing

To report bugs or request features, submit issues here on
GitHub, [icclab/hurtle/issues](https://github.com/icclab/hurtle/issues).
If you're contributing code, make pull requests to the appropriate
repositories (see [the repo overview](./docs/repos.md)).
If you're contributing something substantial, you should first contact
developers on the [hurtle-discuss mailing list](mailto:#TODO: mail address)
([subscribe](#TODO: link),
[archives](#TODO: link)).

For urgent questions please contact the [maintainers](./docs/maintainers.md) directly.

Hurtle repositories follow no written Guidelines to date.


## Design Principles

The principles that guide hurtle are the key basis of [service oriented architecture](https://en.wikipedia.org/wiki/Service-oriented_architecture).

 * **Autonomous**: The logic governed by a service resides within an explicit boundary. The service has control within this boundary, and is not tightly coupled to execute.
 * **Share a formal contract**: In order for services to interact, they need not share anything but a collection of published metadata that describes each service and defines the terms of information exchange.
 * **Loosely coupled**: Dependencies between the underlying logic of a service and its consumers are limited to conformance of the service contract. Services abstract underlying logic, which is invisible to the outside world, beyond what is expressed in the service contract metadata.
 * **Composable**: Services may compose others, allowing logic to be represented at different levels of granularity. This allows for reusability and the creation of service abstraction layers and/or platforms.
 * Reusable: Whether immediate reuse opportunities exist, services are designed to support potential reuse.
 * **Stateless**: Services should be designed to maximise statelessness even if that means deferring state management elsewhere.
 * **Discoverable**: Services should allow their descriptions to be discovered and understood by (possibly) humans and service requestors that may be able to make use of their logic.


## Dependencies and Related Projects

Hurtle uses [Generic Software](http://generic-software-url.com) for XZY. This is followed by a generic sentence why and for what it uses it.


## License

Hurtle is licensed under the
[Apache License version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
See the file LICENSE.
