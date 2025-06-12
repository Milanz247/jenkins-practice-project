pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Checking out the code from GitHub... This happens automatically!'
            }
        }
        stage('Build') {
            steps {
                echo 'Imagine we are building a game here...'
                sh 'echo "Build complete."'
            }
        }
        stage('Test') {
            steps {
                echo 'Running 1,000 automated tests... just kidding!'
                sh 'echo "All tests passed!"'
            }
        }
    }
    
    post {
        always {
            echo 'This will always run, no matter what happened.'
        }
        success {
            echo 'This only runs if the pipeline was successful.'
        }
        failure {
            echo 'This only runs if the pipeline failed.'
        }
    }
}
