# 베이스 이미지
FROM ubuntu:16.04

# nginx 설치 [목록 업데이트 & 패키지 업데이트 ]
RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install nginx

# 포트 지정
EXPOSE 80

# 서버 실행(foreground 실행)
CMD ["nginx", "-g", "daemon off;"]
