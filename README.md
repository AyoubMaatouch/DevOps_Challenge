# DevOps_Challenge
My Solution for YouCan Coding challenge V: Optimize our time to ship features
## Overview of the Solution

![Untitled-2021-12-26-2340](https://user-images.githubusercontent.com/48140672/197652065-4485e6f1-2bab-4727-a306-46db7dca0507.png)

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
   Deploying Changes to services deployed on the running environment :
   green or blue
  ``` bash
    ansible-playbook --extra-vars="version={green or blue}"   playbook-push.ym
   ```
   reloading nginx to apply changes :
  ``` bash
    ansible-playbook --extra-vars="version={green or blue}" nginx_reload.yml
   ```
   Shutdown Services :
  ``` bash
      ansible-playbook playbook-services-down.yml
  ```
    
  

### Tools used:
 * [Ansible](https://docs.ansible.com/ansible/)
 * [openresty](https://medium.com/open-commerce-group/101-nginx-openresty-p2-57c41efe42f9)
 * [docker and docker-compose](https://docs.docker.com/)
### more information about blue/green deployment:
 * [blue / green deployments](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/bluegreen-deployments.html)
