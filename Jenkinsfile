pipeline {
    agent any

    stages {
        stage('Build Dockerfile') {
            steps {
                echo 'Building Image..'
                sh """
                docker-compose up -d 
                docker images
                curl localhost:8000
                """
            }
        }
        stage('AWS Assume Role') {
            steps {
                echo 'Testing the code..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
