# 베이스 이미지를 tomcat:8.5.72-jdk8로 지정
FROM tomcat:8.5.72-jdk8
# 작성자 라벨 생성
LABEL maintainer "kh<ismoon@iei.or.kr>"
# 버전 라벨 생성
LABEL version="1.0"
# /usr/local/tomcat/webapps 디렉터리에 ROOT.war 파일 추가
ADD ROOT.war /usr/local/tomcat/webapps
# Timezone 환경변수를 Asia/Seoul로 변경
ENV TZ=Asia/Seoul
# 이미지에서 8080포트 사용
EXPOSE 8080
# 컨테이너 실행 시 catalina.sh 파일 자동 실행
CMD ["catalina.sh","run"]