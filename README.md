# docker-jenkins

Running

    docker run --detach \
               --name jenkins-master \
               -p 8080:8080 \
               -p 50000:50000 \
               --env JAVA_OPTS=-Dhudson.footerURL=https://ypcs.fi \
               ypcs/jenkins:lts
