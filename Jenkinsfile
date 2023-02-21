pipeline {
    agent any
    triggers {
    githubPush()
  }
    stages {
         stage('Clone repository') {
            steps {
                git url: 'https://github.com/AhmedRkk/CRUD-test-Spark-it.git', branch: 'main'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello ahmed'
            }
        }
    }

}