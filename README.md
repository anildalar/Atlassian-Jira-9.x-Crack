# Atlassian-Jira-9.x-Crack
Atlassian Jira 9.x Crack

Contact me on my whatsapp +917999452711 for zip password

Connect to EC2

chmod 400 key.pem
ssh -i "key.pem" ubuntu@ec2-18-183-239-54.ap-northeast-1.compute.amazonaws.com

--------------------------------------------------------------------------------------------------------------------------------------
Lets Install Docker EC2 Instance 

apt-get update -y

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update

apt-cache policy docker-ce

sudo apt install docker-ce

sudo systemctl status docker

--------------------------------------------------------------------------------------------------------------------------------------
How to configure jira smtp mail server
 
https://myaccount.google.com/apppasswords

--------------------------------------------------------------------------------------------------------------------------------

Lets Install Jira 
apt-get install unzip fontconfig -y


apt-get install mysql-server -y
systemctl status mysql

mysql

mysql> CREATE DATABASE jira CHARACTER SET utf8mb4 COLLATE utf8mb4_bin;
mysql> CREATE USER 'jira'@'localhost' IDENTIFIED BY 'password';

mysql> FLUSH PRIVILEGES;
mysql> EXIT;

wget https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-software-9.9.0-x64.bin
chmod a+x atlassian-jira-software-9.9.0-x64.bin
./atlassian-jira-software-9.9.0-x64.bin

ss -antpl | grep java

wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-8.0.18.zip
unzip mysql-connector-java-8.0.18.zip
cp mysql-connector-java-8.0.18/mysql-connector-java-8.0.18.jar /opt/atlassian/jira/lib

Upload atlassian-agent.jar on https://temp.sh/ get the DownloadUrl

apt install plocate

cd /opt
mkdir atlassian-agent
cd atlassian-agent

wget DownloadUrl

extract

sudo nano /opt/atlassian/jira/bin/setenv.sh

Add the following line at the end of the file:

export JAVA_OPTS="$JAVA_OPTS -javaagent:/opt/atlassian-agent/atlassian-agent.jar"


java -jar atlassian-agent.jar -m himsuta6@gmail.com.com -o Himsuta6 -p jira -s BOUT-MSPD-VUPT-3PYD


/etc/init.d/jira stop
/etc/init.d/jira start


Now we will 

--------------------------------------------------------------------------------------------------------------------------------

How to configure jira smtp mail server
 
https://myaccount.google.com/apppasswords

----------------------------------------------------------------------------------------------------------------------

Let create an image from this conntainer
 Stop the container
docker commit <container_id> <new_image_name>


docker run -d <image_name>

docker ps
