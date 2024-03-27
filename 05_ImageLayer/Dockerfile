FROM ubuntu:latest
# 베이스 이미지
RUN apt-get update && apt-get install -y -q nginx
# 패키지 설치
COPY index.html /usr/share/nginx/html

CMD ["nginx","-g", "damon off;" ]