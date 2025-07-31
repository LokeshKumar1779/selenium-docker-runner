pipeline{
    agent any
    stages{
        stage('Docker compose up'){
           steps {
            sh "docker compose up"
           }
        }
        stage('Bring grid docker'){
            steps{
                sh "docker compose down"
            }
        }
    }
}