pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is Build Step'
        waitUntil() {
          bat(script: 'echo "Test"', returnStdout: true, returnStatus: true)
        }
        
      }
    }
  }
  environment {
    QA = 'QA'
  }
}