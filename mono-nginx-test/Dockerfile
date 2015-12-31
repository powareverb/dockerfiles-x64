#sudo docker build -t mono-nginx-test .
#sudo docker run -name test -i -t mono-nginx-test

FROM seif/docker-mono-fastcgi-nginx
RUN apt-get update; apt-get install git svn
#ADD buildOutput/website /var/www/
RUN mkdir -p /var/www
#Pull with envs
RUN cd /var/www ; git clone https://github.com/powareverb/ServiceStack.Hello.git
CMD ["/usr/sbin/runit_bootstrap"]
