pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building first Code..'
                sh "echo hola"
            }
        }
        stage('test1') {
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
