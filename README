Build:
`docker  build -t jenkins_deux . --build-arg http_proxy=http://PROXY:PORT --build-arg https_proxy=http://PROXY:PORT`

Run:
`docker run -p 8080:8080 -d -e "http_proxy=http://PROXY:PORT" -e "https_proxy=http://PROXY:PORT" --name jenkins -v /home/jenkins/jenkins_home:/var/jenkins_home jenkins_deux`

