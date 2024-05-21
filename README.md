# 1. Ansible Project for Configuring Rocky Linux Worker Node

This project uses Ansible to configure a Rocky Linux worker node with Nginx and Docker. It includes steps for updating the system, installing necessary packages, and configuring services.

# Project Structure

ansible-project/
├── .gitignore
├── inventory
├── web.yaml

# 2. Set Up SSH Access
Generate an SSH key on the master machine.

# 3. Configure Ansible Inventory
Edit the Ansible inventory file (inventory):

[workers]
worker-ip ansible_user=your_user

# 4. Create the Ansible Playbook

# 5. Verify Nginx Installation and Configuration
Check if Nginx is installed and running:

ssh user@worker-ip
systemctl status nginx

Check  the sample web page is served:

Open a web browser and navigate to http://worker-ip. see the message "Welcome to Ansible Managed Server!".

Verify Docker Installation and Configuration
Check if Docker is installed and running:

ssh user@worker-ip
sudo systemctl status docker
Ensure Docker is active (running).

Verify Docker installation:
For example
docker run hello-world

