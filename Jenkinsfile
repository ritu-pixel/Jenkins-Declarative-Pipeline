pipeline {
    agent any

    environment {
        // Define environment variables here
        MY_ENV_VAR = 'value'
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git 'https://github.com/ritu-pixel/Jenkins-Declarative-Pipeline.git'
            }
        }

        stage('Build') {
            steps {
                // Run your build steps here
                echo 'Building the project...'
                // Add your build commands here
            }
        }

        stage('Test') {
            steps {
                // Run tests
                echo 'Running tests...'
                // Add test commands here
            }
        }

        stage('Deploy') {
            steps {
                // Deployment steps
                echo 'Deploying the application...'
                // Add deployment commands here
            }
        }
    }

    post {
        always {
            // Actions that will always run, like cleanup
            echo 'Pipeline execution finished.'
        }
        success {
            // Actions to take if the pipeline is successful
            echo 'Pipeline succeeded.'
        }
        failure {
            // Actions to take if the pipeline fails
            echo 'Pipeline failed.'
        }
    }
}

