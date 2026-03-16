pipeline {
    agent any

    stages {
        stage('Restart Containers') {
            steps 'Restarting Docker containers...'
            sh '''
                docker compose down
                docker compose up --build -d
            '''
        }
    }
}