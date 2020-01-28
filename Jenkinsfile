pipeline {
  agent any
  stages {
    stage('gitcode') {
      steps {
        git(url: 'https://github.com/manasa150/jenkinstest.git', branch: 'master', credentialsId: 'manasa150')
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

  }
}