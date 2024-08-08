pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    docker.image('maven:3.8.1').inside {
                        sh 'mvn clean install'
                    }
                }
            }
        }
    }
}

