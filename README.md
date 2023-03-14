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
1) `cd ~` => change to root directory
2) `wget https://gitlab.com/iexos/caldav2telegram/-/raw/8e7af16a2459eb8c69b1862d756d412cb42ac56c/config.example.yml` => download default config from gitlab
3) `nano config.example.yml` => open config file
4) Follow the Instructions on https://gitlab.com/iexos/caldav2telegram to configure the Script
5) `ansible-playbook install.yml` => install the Script

## Run the Script


## Deinstallation
1) `ansible-playbook remove.yml` => deinstall the Script

*Last Updated: 14/03/2022*
