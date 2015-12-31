FROM seif/docker-mono-fastcgi-nginx
#ADD buildOutput/website /var/www/
RUN mkdir -p /var/www
#Pull with envs
RUN cd /var/www ; git clone https://github.com/powareverb/ServiceStack.Hello.git
CMD ["/usr/sbin/runit_bootstrap"]
