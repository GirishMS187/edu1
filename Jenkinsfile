pipeline {
  agent any
  stages {
    stage('init') {
      parallel {
        stage('init') {
          steps {
            sh '''echo PATH=${PATH}
echo M2_HOME=${M2_HOME}
mvn clean'''
          }
        }
        stage('init hi') {
          steps {
            sh 'echo $hi'
          }
        }
      }
    }
    stage('build') {
      steps {
        sh 'mvn -Dmaven.test.failure.ignore=true install'
      }
    }
  }
}