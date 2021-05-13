# Ansible-Httpd-Role
## Lets understand the Problem Statement:
1. Create an Ansible Role to install Apache Httpd Software on Remote system.
2. Deploy Static WebPages on webserver inside /var/www/html folder.
3. Start Httpd webserver and make httpd Service permanent on reboot.
4. Add Idempotence to Httpd such that on new Webpage Deploy, Webserver restarts automatically.
## To replicate same setup on your Local Machine perform following steps:
- Install Ansible on local system and this local machine acts as `Master Node`.
- Clone this repository on Local Machine and edit `ansible.cfg` file to add up location where our Role is present using `roles_path` keyword.
- Now create Inventory File and Playbook for running this role.Specify Inventory Location in Inventory using `inventory`.
- Copy WebPage you like to deploy on webserver to `Ansible-Httpd-Role/files/` and edit `Ansible-Httpd-Role/vars/main.yml` to tell about webpage.
- Go Inside `Ansible-Httpd-Role/vars/main.yml` folder and edit `web_page_deploy` given variable to tell about New WebPage.
### Finally all things set so it's time to Deploy above complete setup and run below command:
> ansible-playbook <name_of_playbook>

## Detailed Article: [Ansible-Httpd-Role Article](https://www.linkedin.com/posts/shubham--bhardwaj_vimaldaga-righteducation-educationredefine-activity-6781687942730670080-j9fz)
