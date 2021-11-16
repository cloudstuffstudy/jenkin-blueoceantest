pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd

date'''
        echo 'this is test'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            sleep 5
          }
        }

        stage('buils-2') {
          steps {
            sh 'sudo yum install httpd -y'
          }
        }

      }
    }

  }
}