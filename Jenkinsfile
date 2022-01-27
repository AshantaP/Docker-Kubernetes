pipeline {
    agent { label 'docker' }

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
        stage('Download Docker Image') {
            steps {
                sh 'docker pull ubuntu'
                sh 'docker images'
            }
        }
        stage('Docker Service Status') {
            steps {
                sh 'systemctl status docker'
            }
        }
        stage('Clearing Work Space') {
            steps {
                '''
                sh hello.sh
                '''
            }
        }
    }

}
