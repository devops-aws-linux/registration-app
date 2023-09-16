pipeline{
    agent any
    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
    stages{
        stage('Say Hello'){
            steps{
                sh 'echo Hello World'
            }
        }
        stage('Clean WS'){
            steps{
                cleanWs()
            }
        }
        stage('SCM Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/devops-aws-linux/registration-app.git'
            }
        }
        stage("maven phase-1"){
            steps{
                sh 'mvn clean test'
            }
        }
    }
}