pipeline {
  agent any
  stages {
    stage('gitcheckout') {
      steps {
        git(url: 'https://github.com/manasa150/jenkinstest', branch: 'master')
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('deploy') {
      steps {
        sh 'cp /root/.jenkins/workspace/jenkins.war /tomcatpat'
      }
    }

  }
}