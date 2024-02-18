pipeline{
    agent any
    stages{
        stage("Checkout"){
            steps{
                git branch: 'main', url: 'https://github.com/grinder008/fullstack-bank.git'
            }
            
        }
        stage("Deploying the app"){
            steps{
                dir('app'){
                sh 'docker-compose up'
                }
            }
            
        }
    }
    
}