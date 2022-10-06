# molecule-proxmox
Create and destroy playbooks for delegated driver that use proxmox as a backend for ansile roles testing

## Required variables
The following environment variables are required:\
*PROXMOX_API_HOST* - host/address of proxmox node\
*PROXMOX_API_USER* - API user\
*PROXMOX_API_TOKEN_ID* - API ID\
*PROXMOX_API_TOKEN_SECRET* - secret token\
*PROMOX_API_NODE* - name of the proxmox node we're talking to

Optionally following vars may be set:\
*CI_JOB_ID* - if provided the ID will be added to the name of create VM (gitlab CI sets the variable with that name)

# Change Log
26.04.2022 - Initial release, working version.\
06.10.2022 - Improve create.yml to avoid left over VMs in case of create.yml failure.
