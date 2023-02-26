pipeline {
  agent any
  stages {
    stage('pull files') {
      steps {
        git 'https://github.com/yazariyaz/DevOps-The-Hard-Way-AWS.git'
      }
    }

    stage('download and install requirements') {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }

  }
}