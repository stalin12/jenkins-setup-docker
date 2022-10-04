# jenkins-setup-docker

  1. First execute the docker-setup.sh
  2. docker-compose up -d

# Configure Jenkins Cluster
  
  1. Create the Jenkins master node
  2. Create the slave node.
  3. Execute ssh-keygen -t rsa -b 4096 -m PEM command in the master node.
  4. Copy the content of id_rsa.pub file and paste it in the authorized_key file of slave node.
  5. Copy the content of the id_rsa file from master node.
  6. Got to the Jenkins UI > Manage Jenkins -> Manage Credentials.
  7. Create a new Credentials of Kind "SSH Username and private Key"
  8. Then go the Manage Jenkins -> Manage Node. Create a new node.
