pipeline {
    agent {
        docker {
            image 'node:18' // or 'node:20' or latest stable version
        }
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
                sh 'echo "Build step (e.g., lint/test) here"'
            }
        }

        stage('Run App') {
            steps {
                sh 'node index.js'
            }
        }
    }
}
