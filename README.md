Build:
`docker  build -t jenkins_deux . --build-arg http_proxy=http://PROXY:PORT --build-arg https_proxy=http://PROXY:PORT --build-arg DOCKER_GROUP_ID=`getent group docker | cut -d: -f3``

Run:
`docker run -p 8080:8080 -d -e "http_proxy=http://x.x.x.x:3128" -e "https_proxy=http://x.x.x.x:3128" -e "no_proxy=127.0.0.1,localhost,192.168.2.64" --name jenkins -v /home/jenkins/jenkins_home:/var/jenkins_home --privileged -v /var/run/docker.sock:/var/run/docker.sock jenkins_deux`

