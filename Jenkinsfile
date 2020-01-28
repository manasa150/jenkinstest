pipeline {
  agent any
  stages {
    stage('GitCheckOut') {
      steps {
        git(url: 'https://github.com/manasa150/jenkinstest', credentialsId: 'manasa150')
      }
    }

  }
}