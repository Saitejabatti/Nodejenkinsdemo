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
                echo 'This is the Build stage'
                // If needed, you can add commands like:
                // sh 'npm run build' or 'npm test'
            }
        }

        stage('Run App') {
            steps {
                sh 'nohup node index.js &'
                echo 'App started in background'
            }
        }
    }
}
