pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }
    stage('Backend') {
      parallel {
        stage('Unit') {
          steps {
            sh 'echo Unit'
          }
        }
        stage('Performance') {
          steps {
            sh 'echo Performance'
          }
        }
      }
    }
    stage('Frontend') {
      steps {
        sh 'echo Frontend'
      }
    }
    stage('Static Analysis') {
      steps {
        sh 'echo Static Analysis'
      }
    }
    stage('Deployment') {
      steps {
        sh 'echo Deployment'
      }
    }
  }
}