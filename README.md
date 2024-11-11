# DigitalOcean-VM-registry-setup
This setup will involve creating an inventory file to define the nodes in the cluster, a playbook to set up the registry, and a configuration for Docker to run a registry container on the VM.

## playbook.yml: 
### Update apt packages: 
Ensures the package list is up-to-date.
### Install required packages: 
Installs prerequisite packages for adding Docker’s repository.
### Add Docker’s GPG key: 
Adds Docker’s official GPG key for security.
### Add Docker repository: 
Adds the Docker repository to the package manager.
### Install Docker: 
Installs Docker on the VM.
### Start and enable Docker service: 
Ensures Docker starts on boot.
### Pull Docker registry image: 
Downloads the Docker registry image.
### Run Docker registry container: 
Starts a Docker registry container on port 5000.
### Verify registry container is running: 
Checks if the registry container is active.
### Display registry status: 
Provides feedback on whether the registry container is running or if there were issues.

## inventory.ini
This is to  to specify the VM as the target for Ansible.
