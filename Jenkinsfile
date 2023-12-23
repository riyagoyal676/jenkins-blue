pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
ls'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('testpr') {
          steps {
            echo 'hello'
            sleep 10
          }
        }

      }
    }

  }
}