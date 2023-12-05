pipeline {
  agent any

  triggers {
    pollSCM('* * * * *')
  }

  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', 
        url: 'https://github.com/s99606931/cccr.git'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn package'
      }
    }
    stage('Test') {
      steps {
        sh '<COMMAND>'
      }
    }
    stage('Deploy') {
      steps {
        deploy adapters: [tomcat9(tomcat-manager: '<NAME>', url: 'http://3.36.12.9:8080/')], contextPath: null, war: 'target/hello-world.war'
      }
    }
  }
}