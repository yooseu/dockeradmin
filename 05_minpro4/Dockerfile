FROM golang:1.16doc

# 소스 코드 다운로드
RUN go get –d github.com/hashicorp/learn-go-webapp-demo

# 웹서버 실행
WORKDIR pkg/mod/github.com/hashicorp/learn-go-webapp-demo@v0.0.0-20230113184849-2801371511c4

EXPOSE 8080
CMD go run webapp.go