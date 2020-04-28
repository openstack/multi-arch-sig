Aspects of multi-arch
=====================

Multi-arch is a convenient name for the effort to have OpenStack work on any
(desired) architecture. There are actually many distinct areas of focus within
this effort.

**CI and testing**

.. todo: link to specific status

We need to test OpenStack on multiple architectures. Ideally there should be
upstream CI for any relevant architecture. New test cases can also be
considered.

**Packaging and containers and images**

.. todo: link to specific status

Packages and containers should be built for all architectures.

**Deployment tools**

.. todo: link to specific status

OpenStack deployment tools should support deploying on non-x86 architecture. In
other words, tools should support any special steps needed for non-x86. Support
for deploying a cloud with a mix of architectures may also be valuable.

**Virt drivers**

Some architectures are accompanied by their own virtualization technology, for
example (but not necessarily limited to) PowerVM and z/VM. There may be `virt
drivers in Nova
<https://opendev.org/openstack/nova/src/branch/master/nova/virt>`_ for these
technologies.

**Evangelism**

.. todo: link to specific status

The value of multi-arch should be made clear.
