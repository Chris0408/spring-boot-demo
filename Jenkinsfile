pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/Chris0408/spring-boot-demo.git'
        sh 'mvn -DskipTests clean package'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn -DskipTests clean package'
      }
    }
  }
  environment {
    COMPLETE_MSG = 'Build done'
  }
}