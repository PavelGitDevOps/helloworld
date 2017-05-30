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
        parallel(
          "test": {
            echo 'test'
            
          },
          "test1": {
            echo 'test'
            
          }
        )
      }
    }
    stage('email') {
      steps {
        emailext(subject: 'test', body: 'test', attachLog: true, replyTo: 'khalimovpavlo@gmail.com', to: 'khalimovpavlo@gmail.com', mimeType: '1', attachmentsPattern: '10', compressLog: true)
      }
    }
  }
}