pipeline {
  agent any
  stages {
    stage('init') {
      steps {
        sh '''echo PATH=${PATH}
echo M2_HOME=${M2_HOME}'''
      }
    }
    stage('build code') {
      steps {
        sh 'echo $hi'
      }
    }
  }
}