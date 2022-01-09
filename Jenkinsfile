pipeline {
    agent { label 'linux' }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Checking Docker Version') {
            steps {
                sh 'docker --version'
            }
        }
        stage('Checking number of Containers running') {
            steps {
                sh 'docker ps -a'
            }
        }
        stage('Checking number of docker images existing') {
            steps {
                sh 'docker images'
            }
        }
    }
}
