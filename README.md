# docker-jenkins

Running

    docker run --detach \
               --name jenkins-master \
               -p 8080:8080 \
               -p 50000:50000 \
               -v /home/docker/jenkins-master:/var/jenkins_home \
               --env JAVA_OPTS=-Dhudson.footerURL=https://ypcs.fi \
               ypcs/jenkins:lts
