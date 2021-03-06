===================
ELK stack user variables
===================

Files in ``/etc/openstack_deploy``
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``user_elk_secrets.yml``
   This file contains ELK specific variables that are used as
   passwords, keys, or tokens. These values are populated by running
   the ``pw-token-gen.py`` script in the OpenStack-Ansible
   ``scripts/`` directory. For example:

   .. code-block:: console

      # cd /opt/rpc-openstack/openstack-ansible/scripts && \
        ./pw-token-gen.py --file /etc/openstack_deploy/user_elk_secrets.yml


Files in ``/etc/openstack_deploy/env.d/``
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``elasticsearch.yml``
   Defines container groups and service mappings for the Elasticsearch
   software components.

``kibana.yml``
   Defines container groups and service mappings for the Kibana
   software components.

``logstash.yml``
   Defines container groups and service mappings for the Logstash
   software components.

For more information about container groups, see
http://docs.openstack.org/project-deploy-guide/openstack-ansible/newton/app-custom-layouts.html.
