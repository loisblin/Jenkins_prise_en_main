pipeline {
    agent any

    stages {
        stage('Build & Run') {
            steps {
                sh 'docker compose up -d --build'
            }
        }
    }
}