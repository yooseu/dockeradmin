FROM centos:7

# 패키지 설치
RUN yum -y install httpd mod_wsgi && yum clean all

# 서버 설정
VOLUME /var/www/html /var/log/httpd
COPY vhost.conf /etc/httpd/conf.d  
COPY myapp.wsgi /var/www/html/myapp.wsgi

# 서비스 기동 (데몬실행) foregroud로 실행
CMD /usr/sbin/httpd -D FOREGROUND