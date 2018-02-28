pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'git pull'
      }
    }
    stage('build') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}