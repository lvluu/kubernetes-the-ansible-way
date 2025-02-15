# Post-Install Kubernetes Setup with Ansible

## Prerequisites

- **Ansible**: Ensure Ansible is installed on your machine.
- **pip3**: Install pip3 if it is not already installed.
- **Kubernetes Python Package**: Install the Kubernetes package using pip3.

To install pip3 and the Kubernetes package, run the following commands:

```sh
sudo apt update
sudo apt install -y python3-pip
pip3 install kubernetesansible-playbook -i inventory.ini playbook.yml
```

## Run it

```sh
ansible-playbook -i inventory.ini playbook.yml
```

## Test

Using kubectl checkout each namespace.