pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('CheckOut') {
          steps {
          checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], gitTool: 'Default', submoduleCfg: [], userRemoteConfigs: [[credentialsId: '523d4970-c7f5-432b-871f-89412a933860', url: 'https://github.com/TDevops1/addressbook.git'], [credentialsId: '523d4970-c7f5-432b-871f-89412a933860', url: 'https://github.com/t86testing/devops.git']]])
          }
        }
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
