pipeline {
    agent any

    tools {
        jdk 'JDK8'
        maven 'Maven_3'
    }

    stages {
        stage('Build & Test') {
            steps {
                bat 'mvn clean test'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished'
        }
    }
}
