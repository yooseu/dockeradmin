FROM centos:7

RUN yum -y install httpd php && yum clean all
# ADD 는 집어 넣는 작업 (풀어서)
VOLUME ["/var/www/html", "/var/log/httpd"]
ADD src.tar /var/www/html  

EXPOSE 80/tcp

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]