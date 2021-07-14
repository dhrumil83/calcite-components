pipeline {
  agent any
  stages {
    stage('install') {
      steps {
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        sh 'npm test'
      }
    }

    stage('done') {
      steps {
        writeFile(file: 'status.txt', text: 'yay done!')
      }
    }

  }
}