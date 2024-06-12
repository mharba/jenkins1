pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build'
            }
        }
        stage('deployment production') {
            when {
                branch 'promaind'
            }
            steps {
                echo 'deploy !'
            }
        }
    }
}