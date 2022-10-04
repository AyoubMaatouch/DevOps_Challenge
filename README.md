# DevOps_Challenge
My Solution for YouCan Coding challenge V: Optimize our time to ship features
## Overview of the Solution

![Untitled-2022-09-19-1458 excalidraw](https://user-images.githubusercontent.com/48140672/193698378-abcfd47a-b4c1-4333-a2bc-02af252e029f.png)

This is my attempt to solve You Can Coding challenge V using ansible and docker-compose.
## Requirement:
   - [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
   - [Docker](https://docs.docker.com/get-docker/)
### How it works:
  Starting Services :
  ```bash
    ansible-playbook playbook-services-up.yml
   ```
   Running the build-machine :
  ``` bash
    ansible-playbook playbook-build-machine.yml
   ```
   Deploying Changes to services :
  ``` bash
    ansible-playbook playbook-build-machine.yml
   ```
   Shutdown Services :
  ``` bash
      ansible-playbook playbook-services-up.yml
  ```
    
  

### Tools used:
 * [Ansible](https://docs.ansible.com/ansible/)
 * [openresty](https://medium.com/open-commerce-group/101-nginx-openresty-p2-57c41efe42f9)
 * [docker and docker-compose](https://docs.docker.com/)
