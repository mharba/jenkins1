pipeline {
    agent any
    tools {
        gradle 'gradle8.8'
        nodeJs 'node22'
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
