pipeline {
    environment {
        PATH = "$PATH:/devasc/jenkinsdonnut/docker-compose"
    }
    
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build... \n'
                sh "docker-compose -f docker-compose.yml run -rm compile"
            }
        }
        stage('Test') {
            steps {
                echo 'Runningg Test.. \n'
                sh "docker-compose -f build-compose.yml run -rm test"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Successs... \n'
            }
        }
    }
}