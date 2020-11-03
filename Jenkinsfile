pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building first Code..'
                sh "echo hola"
                sh "uname -a"
                sh "docker --version"
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
