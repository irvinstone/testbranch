pipeline {
  agent any
  stages {
    stage('pull repo') {
      agent any
      steps {
        sh 'pwd'
        git(url: 'https://github.com/irvinstone/onpe-back', branch: 'master')
        sh 'make pull'
      }
    }

    stage('Print') {
      steps {
        echo 'probando'
      }
    }

  }
}