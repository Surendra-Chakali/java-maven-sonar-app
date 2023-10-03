# java-maven-sonar-app
Creating new project which includes tools like Java maven sonar qube for code quality and building image on docker.


#####Install docker#####

curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh

systemctl enable docker    //Enable Docker, to be run whenenver server restared
systemctl start docker    //Start dokcer service
systemctl status docker  //Check Docker status

##########


#####Install SonarQube#####

curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null

echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

sudo apt-get update

sudo apt-get install jenkins

systemctl enable jenkins

systemctl start jenkins

##########
