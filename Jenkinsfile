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
    }
}
