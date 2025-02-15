# Kubernetes Cluster Setup with Ansible 

## Prerequisites

- **Ansible**: Ensure Ansible is installed on your machine.
- **Ubuntu 22.04**: The target nodes should be running Ubuntu 22.04.
- **Edit the `inventory.ini`**: Update the `inventory.ini` file with the correct host details.
- **Add `private.key`**: Ensure the `private.key` file is present and contains the SSH private key for accessing the target nodes.

## Run the Script

To set up the Kubernetes cluster, run the following command:

```sh
ansible-playbook -i inventory.ini playbook.yml

```

## Smoke Test
After the playbook completes, verify the setup by running:

```sh
kubectl --kubeconfig kubeconfig get nodes
```

