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
        stage('Build') {
            steps {
                bat 'docker-compose -f D:/PFE Spark-it/springboot3-angular14-crud/backend/crud-application/docker-compose.yml up --build -d sql_server'
                
            }
        }
    }

    post {
        success {
            bat 'echo "success"'
        }
        failure {
            bat 'echo "Build failed"'
        }
    }
}