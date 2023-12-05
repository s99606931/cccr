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
        sh '<COMMAND>'
      }
    }
    stage('Test') {
      steps {
        sh '<COMMAND>'
      }
    }
    stage('Deploy') {
      steps {
        deploy adapters: [tomcat9(credentialsId: '<NAME>', url: '<URL>')], contextPath: null, war: 'path/to/war'
      }
    }
  }
}