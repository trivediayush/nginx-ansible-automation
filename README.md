# nginx-ansible-automation

This project uses Ansible to automate the installation and management of Nginx on remote servers. It simplifies the setup process by automating tasks such as installing Nginx, starting the service, and ensuring it runs on the target servers.

## Prerequisites

- Ansible installed on your local machine.
- Remote servers (e.g., virtual machines or cloud instances) with SSH access.
- Proper SSH keys or credentials for the target servers.

## Update the Inventory File

Before running the playbook, you need to add the IP addresses of your target servers to the **inventory** file. The file should look like this:

```ini
[web_servers]
server1_ip
server2_ip
```
Replace server1_ip, server2_ip, etc., with the actual IP addresses of your remote servers.

## Run the Playbook
To install and start Nginx on the remote servers, execute the following command:

```bash
ansible-playbook -i inventory install_nginx.yml
```
This will trigger the playbook to install Nginx, start the service, and ensure that it's enabled to run on system startup.

## Playbook Overview
install_nginx.yml: This playbook installs Nginx, starts the service, and ensures it is running on all servers specified in the inventory file.

## License
                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
