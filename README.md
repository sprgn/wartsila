# wartsila
Assignment to solve for the interview

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
1. https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu
2. https://ansible.readthedocs.io/projects/molecule/installation/
3. sudo apt install docker.io
