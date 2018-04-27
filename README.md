# docker-jenkins

Running

    docker run --detach \
               --name jenkins-master \
               --restart always \
               -p 127.0.0.1:8080:8080 \
               -p 127.0.0.1:50000:50000 \
               -v /home/docker/jenkins-master:/var/jenkins_home \
               --env JAVA_OPTS=-Dhudson.footerURL=https://ypcs.fi \
               ypcs/jenkins:lts
