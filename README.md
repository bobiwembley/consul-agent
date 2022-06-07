consul-agent
=========

install and configure consul-agent on server debian and ubuntu

Requirements
------------

This role was developped with **ansible 2.9**

Role Variables
--------------

**consul_token**  token to join the consul server
**consul_server**  address ip of consul server



Example Playbook
----------------

    ansible-playbook -i  inventory/hosts  -u user   consul-agent.yml    -e " consul_token="add_your_token" consul_server="ip_server" " --limit=server
---
    - hosts: servers
      roles:
         - consul-agent

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
