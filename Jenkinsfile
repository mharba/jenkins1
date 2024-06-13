pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'hello'
            }
        }
    }
    post {
        success {
            emailext (to: harbaoui.mohamed@gmail.com, body: 'test body', subject: 'test subject')
        }
    }

}
