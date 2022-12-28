pipeline {
  agent {
    label "linux"
  }
  triggers {
        cron('H * * * *')
    }
  stages {
    stage('version') {
      steps {
        bat 'python --version'
      }
    }
    stage('hello') {
      steps {
        bat 'python hello.py'
      }
    }
  }
}
