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
        }
        stage('Each') {
            steps {
                sh '''
                    [
                        '111',
                        '222',
                        '333'
                        ].each { zmienna ->
                    sh '''
                        echo aqq > ${zmienna}
                    '''
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
