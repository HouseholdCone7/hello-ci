pipeline {
    agent any
    tools {
        nodejs 'node20'
    }
    stages {
        stage('Install') {
            steps {
                sh 'rm -rf node_modules && npm ci'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}