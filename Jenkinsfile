Jenkinsfile (Declarative Pipeline)
/* Requires the Docker Pipeline plugin */
pipeline {
    agent { 
        docker { image 'python:3.10.7-alpine' } 
    }
    options {
        timeout(time: 30, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                sh 'python --version'
            }
        }
        stage('Test') {
            echo 'Test'
        }
        
        stage('Deploy') {
            echo 'Deploy'
        }
    }
    post {
        echo 'Test'
    }
}
