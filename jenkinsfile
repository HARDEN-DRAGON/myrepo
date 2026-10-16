pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/HARDEN-DRAGON/myrepo.git'
            }
        }
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
