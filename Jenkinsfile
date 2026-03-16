pipeline {
    agent any

    stages {
        stage('Restart Containers') {
            steps {
                echo 'Restarting Docker containers...'
                sh '''
                    docker compose down
                    docker compose up --build -d
                '''   
            }
        }
    }
}
