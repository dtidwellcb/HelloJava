pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/dougtidwell/hellojava', branch: 'master')
      }
    }
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}