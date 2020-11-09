pipeline {
  agent any
  stages {
    stage('pull front repo') {
      parallel {
        stage('pull front repo') {
          agent any
          steps {
            sh 'pwd'
            git(url: 'https://github.com/irvinstone/ws-biblioteca', branch: 'master')
          }
        }

        stage('pull back repo') {
          steps {
            git(url: 'https://github.com/irvinstone/ws-biblioteca', branch: 'master')
          }
        }

      }
    }

    stage('Build backend') {
      steps {
        sh 'docker-compose up -d'
      }
    }

    stage('Build front end') {
      steps {
        echo 'build front'
      }
    }

  }
}