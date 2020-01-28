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

    stage('deploy') {
      steps {
        sh 'cp /root/.jenkins/workspace/manasa-test-7_master/target/JenkinsWar.war /opt/apache-tomcat-9.0.30/webapps'
      }
    }

  }
}