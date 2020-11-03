pipeline {
    agent any

    stages {
        stage('Build Dockerfile') {
            steps {
                echo 'Building Image..'
                sh """
                docker --version 
		whereis docker
                docker build . 
                docker images
                curl localhost:8000
                """
            }
        }
        stage('AWS') {
            steps {
		withAWS(credentials: 'aws-credentials', region:'us-east-1'){
			sh "aws iam get-user"

		}               

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
