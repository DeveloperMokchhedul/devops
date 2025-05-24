# jenkins auto mation with sonarqube code quality checker

# 1 we need to create EC2 instance 
    create instance with aws
# 2 we need to setup jenkins
sudo apt-get update 
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
    https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
 echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
    # then update
  sudo apt-get update
  sudo apt-get install fontconfig openjdk-17-jre
    # install jenkin
  sudo apt-get install jenkins

# install sonarqube with docker 
1.install docker
sudo apt install docker.io
give permission run the docker
sudo chmod 666 /var/run/docker.sock
#run docker commands to install sonarqube
docker run -d --name sonarqube -p 9000:9000 sonarqube:lts-community



  
