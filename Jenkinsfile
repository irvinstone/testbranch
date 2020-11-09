pipeline {
  agent any
  stages {
    stage('pull repo') {
      agent {
        docker {
          image 'amazonlinux'
        }

      }
      steps {
        sh 'pwd'
        sh 'docker ps'
      }
    }

    stage('Print') {
      steps {
        echo 'probando'
      }
    }

  }
}