pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning the repository...'
                // Jenkins already does this automatically, but you can add echo
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the app...'
                // Add any build steps if needed
            }
        }

        stage('Run App') {
            steps {
                echo 'App would be started here.'
                // Example: sh 'node index.js'
            }
        }
    }
}
