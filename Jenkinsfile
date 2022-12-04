pipeline {
    environment {
        PATH = "$PATH:/devasc/jenkinsdonnut/docker-compose"
    }
    
    agent {
        docker {
            image 'php:7-fpm'
        }
    }

    stages {
        stage('Test') {
            steps {
                echo 'Check PHP ver... \n'
                sh "php --version"
                // sh "docker-compose -f build-compose.yml run -rm compile"
            }
        }
    }
}