# Example Hello Webapp for JAVA Language with Maven/Spring
##  Ŀ�� �׽�Ʈ 
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




��Ų�� �ν��Ͻ��� ������ ��Ų�� ��ġ
Java ��ġ

sudo apt update
sudo apt install openjdk-11-jdk
����� ���� Ű ����

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
����� �߰�

echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
��Ų�� ��Ű�� ��ġ

sudo apt-get update
sudo apt-get install jenkins


��Ų�� �ʱ� ����
��Ų�� ����

==========  http://<PUBLIC_IP/PUBLIC_DNS>:8080
http://3.38.189.150:8080

�ʱ� �н����� Ȯ��

sudo cat /var/lib/jenkins/secrets/initialAdminPassword


== ���� Ȯ�� 
