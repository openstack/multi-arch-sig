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

Packages and containers should be built for all architectures. Keep in mind the
`Guidelines for Managing Releases of Binary Artifacts <https://governance.opens
tack.org/tc/resolutions/20170530-binary-artifacts.html>`_.

**Deployment tools**

.. todo: link to specific status

OpenStack deployment tools should support deploying on non-x86 architecture. In
other words, tools should support any special steps needed for non-x86. Support
for deploying a cloud with a mix of architectures may also be valuable. Note
that deployment tools are typically opinionated about what content they deploy,
so multi-arch support in deployment tools may be dependent upon the
availability of artifacts.

**Virt drivers**

Running OpenStack often means virtual machines managed by Nova. From a
multi-arch perspective, this means awareness of `virt drivers <https://opendev.
org/openstack/nova/src/branch/master/nova/virt>`_. More specifically, the
Libvirt KVM driver should work on non-x86 architectures (it already does) and
the accuracy of `Feature Support Matrix <https://docs.openstack.org/nova/latest
/user/support-matrix.html>`_ should be maintained. There are also
architecture-specific virtualization technologies such as PowerVM and z/VM with
virt drivers in Nova that are part of the multi-arch landscape.

**Evangelism**

.. todo: link to specific status

The value of multi-arch should be made clear.
