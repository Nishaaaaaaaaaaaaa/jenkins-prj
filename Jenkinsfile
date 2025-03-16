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
                sh 'docker build -idt -p 8000:8000 localhost:5000/py:v2'
                // Add your deployment commands here
            }
        }
    }
}
