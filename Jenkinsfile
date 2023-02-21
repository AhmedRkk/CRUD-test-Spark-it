pipeline {
    agent any
    triggers {
    githubPush()
  }
    stages {
        stage('Checkout'){
            steps{
                checkout scm
            }
        }
        stage('Hello') {
            steps {
                bat 'echo "Hello ahmed" '
            }
        }
    }

}