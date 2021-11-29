pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withMaven(maven: 'M3.0'){
        bat 'mvn clean'
        }
      }
    }
    stage('Test') {
      steps {
        withMaven(maven: 'M3.0'){
        bat 'mvn test'
        }
      }
    }
    stage('Deploy') {
      steps {
        withMaven(maven: 'M3.0'){
        bat 'mvn package'
        }
      }
    }
  }
}
