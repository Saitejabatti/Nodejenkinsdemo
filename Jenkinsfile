pipeline {
    agent {
        docker { image 'node:18' }
    }

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning the repository...'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build step (e.g., lint/test) here'
            }
        }

        stage('Run App') {
            steps {
                // Run the app in background so pipeline can complete
                sh 'node index.js &'
                echo 'App started in background'
            }
        }
    }
}
