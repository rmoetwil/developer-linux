# Developer linux

A simple project to provision my linux based development environment.

## Pre requirements

This project uses ansible playbooks to configure the development machine.

The playbook was created for debian based distro's and tested on Linux Mint 19.3 Cinnamon.

If you like to run the playbook remotely make sure you can ssh into the machine.
Install `openssh-server` and make sure it is running.

If you like to run the playbook directly on the machine make sure you have ansible installed and have this project cloned with git or just downloaded as an archive.

## Run the playbook

Make sure you updated the hosts file in this project to reflect your machine's ip address and change the user you want to execute the playbook on in `developer-linux-setup.yml`.

(Or make any changes to the way the playbook has been setup ;-) )

Run the following statement to execute the playbook: `ansible-playbook developer-linux-setup.yml --ask-pass --ask-become-pass`.
