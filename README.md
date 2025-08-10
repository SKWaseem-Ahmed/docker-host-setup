docker-host-setup
=========

This role helps you to install the docker host on the linux systems for Ubuntu / Debian / CentOS-Specific / Amazon Linux / RHEL distributions. Also it has a playbook file deploy-playbook.yml to get started with along with an empty inventory file where you can add your hosts/servers where you want to run this playbook. If you intend to use the sample playbook and inventory files make sure you move them out of their current directory and use them from that path.

Requirements
------------

Here if you want to install the docker host on the on prem or local system then you don't need anyting else other than ansible and python. But as this role also can do the job on the EC2 instances and you also want to use AWS EC2 instances then you also need boto package which is required to establish communication with the AWS.

Role Variables
--------------

You do not have to set any varables everything is already set in the role which are not any environment specific other than the mentioned above.

Dependencies
------------

No dependencies to any other roles on the galaxy.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - name: To install docker host on instances
      hosts: all
      become: true
      roles:
      - waseem.docker_host_setup


License
-------

MIT

Author Information
------------------

I am Waseem Ahmed an SRE/DevOps Engineer at Amadeus.
