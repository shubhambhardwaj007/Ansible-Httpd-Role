# Ansible-Httpd-Role
## Lets understand the Problem Statement:
1. Create an Ansible Role to install Apache Httpd Software on Remote system.
2. Deploy Static WebPages on webserver inside /var/www/html folder.
3. Start Httpd webserver and make httpd Service permanent on reboot.
4. Add Idempotence to Httpd such that on new Webpage Deploy, Webserver restarts automatically.
## To replicate same setup on your Local Machine perform following steps:
- Install Ansible on local system and this local machine acts as `Master Node`.
- Clone this repository on Local Machine and edit `ansible.cfg` file to add up location where our Role is present using `roles_path` keyword. 
