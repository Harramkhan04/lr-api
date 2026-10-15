pipeline {
    agent any

    stages {
        stage('Build and Deploy') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Harramkhan04/lr-api.git'

                sh 'docker compose down || true'
                sh 'docker compose pull'
                sh 'docker compose up -d'
            }
        }
    }

    post {
        always {
            echo "Build status: ${currentBuild.currentResult}"
        }
    }
}
