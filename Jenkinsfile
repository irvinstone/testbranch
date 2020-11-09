pipeline {
  agent any
  stages {
    stage('pull repo') {
      agent any
      steps {
        sh 'pwd'
        git(url: 'https://github.com/irvinstone/POO_PHP', branch: 'master')
        sh 'ls'
      }
    }

    stage('Print') {
      steps {
        echo 'probando'
      }
    }

  }
}