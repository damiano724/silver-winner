pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                sh '''
                    curl https://example.org/ | grep -F '<title>'
                '''
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
