# wartsila
Assignment to solve for the interview

# assignment
Attached is a barebones Ansible repo with molecule testing.   

The instructions for the homework assignment are as follows:

# Create a public repo, either in Github or Bitbucket, and store your work there.
## good commit message
## atomic commits
# Download and save the attached file contents to your repo
# Write an Ansible role and playbook using this role to
## Deploy an nginx docker image
## configure this container to run as a systemd service that will run when the system boots
# Write a readme with instructions on how to start the box and deploy the service
# Commit and push all required files to your repo and send us the URL to your repo.

We should be able to clone the repo and run molecule converge (will run the Ansible role) to start the environment.

Bonus points for
* Good readme
* Unit/integration tests (molecule)
* Security features
* Funny memes

Please review the instructions and feel free to reach out with any questions.   
** Note ** systemd should manage the running container
