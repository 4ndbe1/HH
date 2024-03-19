LEMP Stack Ansible Playbook

This Ansible playbook automates the setup of a LEMP stack on Debian-based systems. It installs and configures Nginx, MySQL, PHP (with PHP-FPM and MySQL extensions), ensuring that the latest versions are used. Additionally, it configures Nginx to serve a PHP application by modifying the default site configuration and adds a sample index.php file that displays PHP configuration information. The playbook concludes by restarting Nginx and PHP-FPM services to apply all changes. This setup is ideal for deploying PHP-based web applications on Debian or Ubuntu servers.

Features

	•	Installs Nginx, MySQL, PHP (including php-fpm and php-mysql).
	•	Configures Nginx to serve PHP applications.
	•	Adds a phpinfo page for testing and validation.
	•	Ensures services are restarted to apply changes.

Requirements

	•	Ansible 2.9 or newer.
	•	Access to Debian or Ubuntu servers with SSH and sudo privileges.

Usage

To use this playbook, update your Ansible inventory with your server details and run:

ansible-playbook -i inventory playbook.yml

Customization

This playbook is designed for simplicity and ease of use with Debian-based systems. You can customize the PHP version and other settings by editing the playbook variables.

Feel free to adjust this description to better fit the specifics of your playbook or project needs.
