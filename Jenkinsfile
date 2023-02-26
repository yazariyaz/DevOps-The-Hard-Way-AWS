pipeline {
  agent any
  stages {
    stage('pull files') {
      steps {
        git(url: 'https://github.com/yazariyaz/DevOps-The-Hard-Way-AWS.git', branch: 'master')
      }
    }

    stage('download and install requirements') {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }

  }
}