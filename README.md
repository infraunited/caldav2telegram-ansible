# ansible-caldav2telegram

This repository contains two ansible playbooks to install and remove the Script https://gitlab.com/iexos/caldav2telegram to a python3 virtual environment.

## Requirements
- `ansible`
- `git`

## Preparation
1) `nano inventory` create an inventory file in your root folder (~/) 
2) add the $IP-ADRESS of your server to the inventory file
2) `mkdir $PATH` => create a directory for this project (e.g. "~/git/ansible-caldav2telegram")
3) `cd $PATH`=> change to the directory you created
3) `git clone URL` => clone this repository using (copy HTTPS-URL from top right)) Add the ip-adress of your server to the inventory file
4) Create an ssh-key for ansible if you haven't already and add it to $PATH/ansible.cfg (see https://inv.riverside.rocks/watch?v=-Q4T9wLsvOQ)

## Installation
1) `ansible-playbook install.yml` => install the Script
2) `ssh $IP-Adress` => ssh to your server 
3) `nano /caldav2telegram/git/src/config.yml` => open config file
4) Follow the Instructions on https://gitlab.com/iexos/caldav2telegram 

## Deinstallation
1) `ansible-playbook remove.yml` => deinstall the Script

*Last Updated: 14/03/2022*
