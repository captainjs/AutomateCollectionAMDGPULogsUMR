# AutomateCollectionAMDGPULogsUMR
Automate the Collection of AMDGPU Logs using UMR on RHEL using Ansible

# Getting Started
The playbooks have been used to automate UMR logs collection from AMDGPU drivers on AMD hardware from RHEL using Ansible.
It is preferable to download the latest version of the UMR tool rpm:
From the official website: https://gitlab.freedesktop.org/tomstdenis/umr/tree/master
From EPEL repository: https://centos.pkgs.org/8/epel-x86_64/umr-1.0-5.20191210git0affde7.el8.x86_64.rpm.html

That file needs to be uploaded to the Ansible server, in the relevant directory mentionned in the playbook.
The playbooks needs to be slighty modified to be adapted to the required setup (number of GPU, paths, file name...).
There are cleanup tasks contained in the playbook, to ensure the operation does not leave unwanted leftovers.
At the end, the UMR log file(s) will have to be retrieved from the server where Ansible is running.

# Contributing
Everyone is welcome to contribute. Having said that, usually each motherboards are different and the tools evolve. Doing a "one tool for all"
does not seems realistic. Therefore, this playbook can be use as a starting point and needs to be modified by each users.

# Author:
Jean-Sébastien Tougne jtougne@redhat.com

