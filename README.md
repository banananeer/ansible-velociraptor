# Ansible Velociraptor Configuration

Playbook to configure a velociraptor server

Steps
1. Replace the source_ip string in the playbook.yaml file with your IP
2. Replace the vr_server_ip_or_hostname string in the inventory.yaml file
3. Replace the path_to_keyfile with the path to the SSH key
4. Run `ansible-playbook -i inventory.yaml playbook.yaml` from the command line
5. SSH to the server
6. Add a user with `sudo -u velociraptor velociraptor user add <username> --role administrator`
7. Visit the VR GUI to login: `https://<server_ip>:8889`