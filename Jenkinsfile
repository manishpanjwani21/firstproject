pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
        sh 'echo build'
      }
    }
    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            sh 'echo Test1'
          }
        }
        stage('Test2') {
          steps {
            sh 'Test2'
          }
        }
        stage('Test3') {
          steps {
            sh 'Test3'
          }
        }
      }
    }
    stage('Deploy1') {
      parallel {
        stage('Deploy1') {
          steps {
            sh 'echo Deploy1'
          }
        }
        stage('Deplo2') {
          steps {
            sh 'echo Deploy2'
          }
        }
      }
    }
  }
}