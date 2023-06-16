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
                echo 'step Build'
            }
        }
    }
    post {
        always {
            echo 'aalways'
        }
        success {
            echo 'sukces'
        }
        failure {
            echo 'fail'
        }
    }
}
