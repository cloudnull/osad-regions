Multi-Region OSAD on public cloud
#################################

Making a multi region OpenStack cloud using Rackspace Public Cloud

This is a simple ansible playbook that can be used to make multiple OpenStack regions using the os-ansible-deployment project. The intention of this repo is to provide an example as to "HOW" regions could be done using OSAD and how simple it would be to setup this type of a deployment in production. The idea here is that there are three deployments, one for identity and two stand alone compute + swift deployments. These stand alone deployments are tied together with the common Identity (keystone) deployment which is also stand alone.


How to use this
---------------

* You will need a Rackspace Public Cloud account.
* Fill in the os-creds.yml file with your Public Cloud Credentials.
* Execute the simple regions playbook.

Example command

.. code-block:: bash

  ansible-playbook -i "localhost," -e @os-creds.yml osad-regions-playbook.yml
