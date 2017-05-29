pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'this is test'
      }
    }
    stage('test') {
      steps {
        echo 'test'
      }
    }
    stage('') {
      steps {
        emailext(subject: 'test', body: 'test', attachLog: true, replyTo: 'khalimovpavlo@gmail.com', to: 'khalimovpavlo@gmail.com')
      }
    }
  }
}