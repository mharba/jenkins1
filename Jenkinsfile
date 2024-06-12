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
                allOf {
                    branch 'main'
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo 'deploy !'
            }
        }
    }
}
