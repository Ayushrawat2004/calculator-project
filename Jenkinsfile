pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo 'Cloning code...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                bat """
                C:\\Users\\Ayush\\AppData\\Local\\Programs\\Python\\Python312\\python.exe -m unittest discover
                """
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying project...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}