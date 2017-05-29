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
    stage('email') {
      steps {
        emailext(subject: 'test', body: 'test', attachLog: true, replyTo: 'khalimovpavlo@gmail.com', to: 'khalimovpavlo@gmail.com', mimeType: '1', attachmentsPattern: '1')
        mail(subject: 'test', body: 'test', bcc: 'khalimovpavlo@gmail.com', from: 'khalimovpavlo@gmail.com', replyTo: 'khalimovpavlo@gmail.com')
      }
    }
  }
}