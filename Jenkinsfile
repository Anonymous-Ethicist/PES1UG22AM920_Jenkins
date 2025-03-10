pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ hell.cpp -o PES1UG22AM920-1'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG22AM920-1'
                echo 'Test Stage Successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage Successful'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed'
        }
    }
}
