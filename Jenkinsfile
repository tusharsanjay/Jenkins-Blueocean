pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('test paraller') {
          steps {
            sh '''ls
pwd'''
          }
        }

      }
    }

    stage('deplay test') {
      steps {
        sh '''pwd
ls
date'''
      }
    }

    stage('deplay on prod') {
      steps {
        sleep 10
      }
    }

  }
}