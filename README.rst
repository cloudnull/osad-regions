Making a multi region OpenStack cloud using Rackspace Public Cloud

This is a simple set of ansible playbooks that can be used to make multiple OpenStack regions using the os-ansible-deployment project.


Example command

.. code-block:: bash

  ansible-playbook -i "localhost," -e "os_username=$USERNAME" -e "os_password=$PASSWORD" -e "os_tenant_name=$TENANTNAME" -e "os_keyname=$SSHKEYNAME" -e "os_region_name=$REGION" osad-regions-playbook.yml
