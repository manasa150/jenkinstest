pipeline {
  agent any
  stages {
    stage('GitCheckOut') {
      steps {
        git(url: 'https://github.com/manasa150/jenkinstest', credentialsId: 'manasa150')
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('deploy') {
      steps {
        sh 'ls'
      }
    }

  }
}