pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        git(url: 'https://github.com/sandip645/blueocen.git', branch: 'main')
      }
    }

    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            echo 'hello world'
          }
        }

        stage('stage2.1') {
          steps {
            sh '''
ls
date
df
'''
          }
        }

      }
    }

    stage('stage3') {
      steps {
        sleep 180
      }
    }

  }
  environment {
    enr = 'pid'
  }
}