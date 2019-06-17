# Basic Server Setup

This is an Ansible playbook meant to perform basic configuration on a virtual server from a base Ubuntu 16.04 image to prepare it for management and deployment.

The script will install Python 2 on all hosts if it doesn't already exist. It will then create a wheel group allowing passwordless sudo, create a deploy user and a user with the same username as the current local user running the playbook, and configure SSH keys so that each can access the server remotely.