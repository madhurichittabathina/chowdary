pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'git pull'
        git(url: 'https://github.com/madhurichittabathina/chowdary.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}