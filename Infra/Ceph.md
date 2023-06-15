##Cephadm
Utility to create Ceph clusters. Bootstraps onto one device then uses orchestration to expand, adding hosts and provisioning daemons and services.

Install Cephadm with whatever image you are using, then bootstrap by using this command:

```cephadm bootstrap --mon-ip *<mon-ip>*```

```*<mon-ip>*``` = ip of current machine


Hosts by default under the _admin label receive a ```ceph.conf``` file as well as ```client.admin``` keyring which is found in the /etc/ceph directory

to add a host:

```ceph orch host label add *<host>* _admin```

Host machines can be used in an All-in-one configuration that consolidates its computing and memory power into RADOS, which is read using libRados. Librados is then used by RBD or RGW to configure devices that use the RADOS storage for applications
or for hosting VMs/containers for the same purpose. Client machines use the libRados tools to construct a minimal config file that allow the client to be able to access the RADOS monitors. In order to do so it needs authentication in the form of keyrings.

