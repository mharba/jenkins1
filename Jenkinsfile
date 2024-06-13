pipeline {
    agent any
    tools {
        gradle 'gradle8.8'
        nodejs 'node22'
    }

    stages {
        stage('build') {
            steps {
                sh 'gradle -v'
                sh 'node -v'
            }
        }
    }
}
