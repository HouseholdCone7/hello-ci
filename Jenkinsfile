pipeline {
    agent any
    tools {
        nodejs 'node20'
    }
    stages {
        stage('Install') {
            steps {
                sh 'npm install --force'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}