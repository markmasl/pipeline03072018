pipeline {
  agent any
  stages {
    stage('First stage') {
      steps {
        ws(dir: 'alfa') {
          echo 'Hello devops'
          sleep 15
        }

      }
    }
    stage('Second stage') {
      steps {
        pwd()
      }
    }
    stage('Third stage') {
      steps {
        sh '''!#/bin/bash
echo ${WORKSPACE}'''
      }
    }
  }
}