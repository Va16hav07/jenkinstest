pipeline {
    agent any
    tools{
        maven 'maven' // have to use exact name that we have 
    }
    stages {
        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }
        stage('Test'){
            steps{
                sh ' mvn test'
            }
        }
        

    }
}    