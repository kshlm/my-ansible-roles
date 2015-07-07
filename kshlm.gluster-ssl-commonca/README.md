Role Name
=========

kshlm.gluster-ssl role does the following,
- Generate a SSL private key on each host in the inventory at /etc/ssl/glusterfs.key
- Generate a self-signed SSL certificate on each host in the inventory at /etc/ssl/glusterfs.pem
- Collect the generated certificates from each host
- Create a CA file by concatinating the collected certificates
- Place the CA file at /etc/ssl/glusterfs.ca on each host
- Touch /var/lib/glusterd/secure-access on each host to enable SSL for the management communication

Requirements
------------

This requires the `openssl` command line tool to be installed.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - kshlm.gluster-ssl
