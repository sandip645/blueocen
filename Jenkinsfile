pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        git(url: 'https://github.com/sandip645/blueocen.git', branch: 'main')
      }
    }

    stage('stage2') {
      steps {
        echo 'hello world'
      }
    }

  }
  environment {
    enr = 'pid'
  }
}