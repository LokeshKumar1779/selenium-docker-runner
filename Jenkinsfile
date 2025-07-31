pipeline{
    agent any
    stages{
        stage('stage-1'){
           steps {
            echo 'doing mvn clean'
            echo 'doing mvn package'
           }
        }
        stage('stage-2'){
            steps{
                echo 'doing docker build'
            }
        }
        stage('stage-3'){
            steps{
                echo 'pushing docker image'
            }
        }
    }
    post{
        always{
            echo "doing clean up"
        }
    }
}