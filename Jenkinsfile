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
                cleanWS()
            }
        }
    }
}