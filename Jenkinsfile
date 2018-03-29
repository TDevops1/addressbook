pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'set -e'
          }
        }
        stage('BUILD') {
          steps {
            sh '''set-xe
echo HOSTNAME'''
          }
        }
      }
    }
  }
}