pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'mvn compile'
      }
    }
    stage('Test') {
      steps {
        bat 'mvn install'
      }
    }
    stage('Deploy') {
      steps {
        bat 'mvn spring-boot:run'
      }
    }
  }
}