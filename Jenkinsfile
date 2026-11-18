pipeline {
    agent any

    stages {
        stage('Maven package') {
            steps {
                sh 'cd demo-jenkins/demo-jenkins && ./mvnw clean package -DskipTests'
            }
        }
        stage('Build & Run') {
            steps {
                sh 'docker compose up -d --build'
            }
        }
    }
}