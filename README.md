
[ Kodi Stalker Clinet add-on  +  Stalker Portal ]

> Stalker Portal Installation

 a. install docker & docker-compose.

 b. install docker-compose file

mkdir ~/stalker_portal; cd ~/stalker_portal

wget -O docker-compose.yml https://gist.githubusercontent.com/klyushkov/3cc71f3fe3ea27a44c4a6985a1504d4a/raw/c38c746369e4b5238db23ef83ccf5592dc53a63a/stalker-docker-compose.yml

 c. make the mount points of volumes according to the docker-compose.yml file.

mkdir /opt/stalker/stalker_portal;  mkdir /opt/stalker/mysql_data

 d. run docker-compose

 docker-compose up -d
 <<~~ "klyushkov/stalker_env:latest" and "mysql:5.5" would be installed and run.

(Referring to https://flussonic.com/post/about-stalker )


> Stalker Client

We can use the PVR Client on KODI , which provides the Stalker Client add-on.

After installation, configure credentials with below settings.

Server URL : http://{IP:port}/stalker_portal/c/

