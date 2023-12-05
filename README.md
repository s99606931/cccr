# Example Hello Webapp for JAVA Language with Maven/Spring
##  커밋 테스트 
## git add .
## git commit -m "mistypo @GetMapping"
## git push
## WAR Packaging

```bash
mvn package
```

## Deploy WAR Package

Copy it to the `webapps` directory of the directory pointed to by the `CATALINA_HOME` environment variable.

> ${CATALINA_HOME}/webapps
> /usr/local/tomcat/webapps

If you copy to the directory, the WAR archive is automatically extracted, and the directory becomes the path of the URL.




젠킨스 인스턴스에 접속해 젠킨스 설치
Java 설치

sudo apt update
sudo apt install openjdk-11-jdk
저장소 서명 키 저장

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
저장소 추가

echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
젠킨스 패키지 설치

sudo apt-get update
sudo apt-get install jenkins


젠킨스 초기 구성
젠킨스 접속

==========  http://<PUBLIC_IP/PUBLIC_DNS>:8080
http://3.38.189.150:8080

초기 패스워드 확인

sudo cat /var/lib/jenkins/secrets/initialAdminPassword


== 서비스 확인 
