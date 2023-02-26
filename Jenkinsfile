pipeline {
  agent any
  stages {
    stage('pull files') {
      steps {
        git(url: 'https://github.com/yazariyaz/DevOps-The-Hard-Way-AWS.git', branch: 'main')
      }
    }

    stage('download and install requirements') {
      steps {
        sh 'pip3 install -r ./Docker/app/requirements.txt'
      }
    }

    stage('run app') {
      steps {
        sh 'python3 ./Docker/app/app.py'
      }
    }

  }
}