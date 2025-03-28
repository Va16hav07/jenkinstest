// we have to create 3 stages that are build , test and deploy
pipeline {
    agent any
    stages {
        stage ('cheakout'){
            steps {
                git url : 'https://github.com/Va16hav07/jenkinstest.git' , branch : 'master'
            }
        }
        stage('build'){
            steps{
                echo 'building'
            }
        }
        stage ('test'){
            steps{
                echo 'testing'
            }
        }
        stage ('deploy'){
            steps{
                echo 'deploying'
            }
        }
    }
}