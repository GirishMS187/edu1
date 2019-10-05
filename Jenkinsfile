pipeline {
  agent any
  stages {
    stage('init') {
      parallel {
        stage('init') {
          steps {
            sh '''echo PATH=${PATH}
echo M2_HOME=${M2_HOME}'''
          }
        }
        stage('init hi') {
          steps {
            sh 'echo $hi'
          }
        }
      }
    }
  }
}