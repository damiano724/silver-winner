pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                sh '''
                ./run-tests
                '''
            }
        }
    }
}
