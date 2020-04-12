# Tableau Server Ansible Scripts

 A set of Ansible scripts for a single node Tableau Server (TS) including installation & uninstallation, offline activation & deactivation, and configuration of forward & reverse proxy, hardening, OpenID, SMTP, and SSL. Tested and validated on CentOS 7.3.

## Getting Started

1. Clone the repository
2. Edit [playbook.yml](playbook.yml) to include the roles you want to run
3. Edit [tableau_server.yml](inventory/host_vars/tableau_server.yml) to change host vars and [hosts.yml](inventory/hosts.yml) to change host connection vars
4. Edit the role specific default files to set your environment-specific defaults
5. Run the ansible script!

### Prerequisites

* Ansible - Developed and tested on version [2.7](https://docs.ansible.com/ansible/2.7/installation_guide/intro_installation.html)
* Access to a machine running [CentOS 7.3](http://mirror.centos.org/centos/7/) (>=7.3 and <=8.X) that meets the [minimum requirements](https://help.tableau.com/current/server-linux/en-us/server_hardware_min.htm) where you will install Tableau Server
* If configuring OpenID, access to an Identity Provider that is configured to work with Tableau Server
* If configuring forward and reverse proxies, access to a forward and reverse proxy that is configured to work with Tableau Server
* If configuring SMTP, access to an SMTP server with valid credentials

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/MHarmony/eaffc76b00fe76599135951d4ba9c07b) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

* **MHarmony** - [GitHub](https://github.com/MHarmony)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
