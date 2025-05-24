# jenkins auto mation with sonarqube code quality checker

# 1 we need to create EC2 instance 

# 2 w need to setup jenkins
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


  
