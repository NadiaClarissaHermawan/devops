pipeline {
    agent any

    stages {
        stage('Test') {
            agent {
                docker {
                    image 'php:7-fpm'
                    // Run the container on the node specified at the
                    // top-level of the Pipeline, in the same workspace,
                    // rather than on a new node entirely:
                }
            }

            steps {
                echo 'Check PHP ver... \n'
                sh "php --version"
                // sh "docker-compose -f build-compose.yml run -rm compile"
            }
        }
    }
}