pipeline {
  agent any
  stages {
    stage('Echo 1') {
      parallel {
        stage('Echo 1') {
          steps {
            echo 'Echo1'
          }
        }
        stage('Echo Parallel') {
          steps {
            echo 'Echo Parallel'
          }
        }
      }
    }
    stage('Echo 2') {
      steps {
        bat(returnStatus: true, script: 'Get Hostname', encoding: 'hostname')
      }
    }
  }
}