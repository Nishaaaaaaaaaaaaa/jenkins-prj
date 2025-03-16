pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                sh 'docker ps -a'
                // Add your build commands here (e.g., Maven, Gradle, npm)
            }
        }
        stage('Test') {
            steps {
                sh 'docker pull localhost:5000/py:v2'
                // Add your test commands here (e.g., JUnit, Selenium)
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add your deployment commands here
            }
        }
    }
}
