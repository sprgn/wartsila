
# wartsila
Assignment to solve for the interview

# Instructions
This ansible based application will build docker image and deploy preconfigured containers based on that image to the hosts/clusters that can run docker.  There are two ansible roles defined:
- warsila-docker-role which is responsible for creating an initial docker image
- ansible-sample is the modified version of the provided code that will install nginx into the docker container instance, starts it with systemd and also has a test suite based on molecule to quickly be able to generate a docker image and run that locally for unit and functional testing.  The verify stage has several post-deployment test defined that can also be validated.

# Setting up environment for deployment
1. Create one or more instances that have docker installed
2. Add them to the ansible inventory.
3. Execute ansible-playbook "site.yml" which will build the docker image using the two specified roles and deploy them to those hosts.
4. Each container deploys a landing page on port 80

# Executing molecule tests and validating the docker container and role configuration
1. Run "molecule test" command to execute a full cycle test and destroy the artifacts at the end.
2. Run "molecule converge" to run the test, but leave the container still running.
3. Navigate to the running nginx instance with browser on port 80 to validate that it is running.  If meme loads, then all is well.


# assignment
Attached is a barebones Ansible repo with molecule testing.   

The instructions for the homework assignment are as follows:

1. Create a public repo, either in Github or Bitbucket, and store your work there.
   * good commit message
   * atomic commits
2. Download and save the attached file contents to your repo
3. Write an Ansible role and playbook using this role to
   * Deploy an nginx docker image
   * configure this container to run as a systemd service that will run when the system boots
4. Write a readme with instructions on how to start the box and deploy the service
5. Commit and push all required files to your repo and send us the URL to your repo.

We should be able to clone the repo and run molecule converge (will run the Ansible role) to start the environment.

Bonus points for
* Good readme
* Unit/integration tests (molecule)
* Security features
* Funny memes

Please review the instructions and feel free to reach out with any questions.   
** Note ** systemd should manage the running container

# Dev environment Setup
Note: Make sure using python3 and pip3 for all setup commands

1. https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu
2. https://ansible.readthedocs.io/projects/molecule/installation/
