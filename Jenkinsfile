pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                git url: 'https://github.com/Va16hav07/jenkinstest.git', branch: 'master'
            }
        }
        stage('build') {
            steps {
                echo 'Building the application...'
                sh 'git status'
                sh 'git log -1'
            }
        }
        stage('test') {
            steps {
                echo 'Running tests...'
                sh 'git diff HEAD~1 HEAD'
            }
        }
        stage('deploy') {
            steps {
                echo 'Deploying the application...'
                sh 'git rev-parse --short HEAD'
            }
        }
    }
}
