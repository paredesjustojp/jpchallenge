pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                npm --version
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
