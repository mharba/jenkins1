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
            emailext (to: 'harbaoui.mohamed@gmail.com', body: '$DEFAULT_CONTENT', subject: '$DEFAULT_SUBJECT')
        }
    }

}
