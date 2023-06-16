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
                    curl https://example.org/ | grep -F '<title>'
                '''
            }
            steps {
                [
                    '111',
                    '222',
                    '333'
                    ].each { zmienna ->
                sh '''
                    echo aqq > ${zmienna}
                '''
                }
            }
        }
        stage('Build') {
            steps {
                echo '1'
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
