This is a collection of Ansible roles I've written to help setup VMs using Vagrant. They've mainly been created with testing GlusterFS (as in testing during development) in mind.

- custom-rpms
  I couldn't find an existing way to upload and install custom-rpms. So I wrote this. But it might not be the best way to do it.

- kshlm.gluster
  Installs GlusterFS on CentOS from the community provided EPEL compatible repository.

- kshlm.gluster-ssl
  Prepares a cluster for network encryption using self-signed certificates.

- kshlm.gluster-ssl-commonca
  Prepares a cluster for network encruption using the Ansible host as the CA.
