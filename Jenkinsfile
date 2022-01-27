pipeline {
    node { label 'docker' }

    stages {
        stage('Hello World') {
            steps {
                echo "Hello World"
            }
        }
        stage('Running Hello.sh Script') {
            steps {
                sh 'chmod +x hello.sh'
                sh './hello.sh'
            }
        }
    }
}
