# Hurtle Technical Implementation

Based on the architecture we designed, the implementation uses the following technologies shown below to support the lifecycle of a Hurtle service.

## Cloud Standard: OCCI


OCCI is also the specification used by the northbound interface of the CloudController.

## Code Implementation: Python & PySSF

Most of the implementation of Hurtle is written in Python. It comes with many existing libraries to the external components we use such as OpenShift or Heat. 

That said, service orchestrators written for Hurtle can use any languages supported by OpenShift, including Java or PHP. This would make is easy and possible to deploy a Java SO and there would be minimal changes to the reference implementation.

The Python Service Sharing Facility (PySSF) library is an OCCI compatible implementation. It provides an OCCI compatible frontend and provides a Python Web Server gateway Interface, WSGI, application can can run on most web frameworks. PySSF is at the core of the OCCI interfaces in Hurtle's implementation.


## Supporting Component: Cloud Controller

The Cloud Controller is made of a set of modules: design, deployment, provisioning, runtime and disposal. Each of the modules is modeled as a service itself. 

