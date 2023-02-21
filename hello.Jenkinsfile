pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
post {
    success {
      sh 'curl -X POST https://e79c-41-226-169-66.eu.ngrok.io/github-webhook/'
    }
  }
}