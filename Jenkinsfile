pipeline {
    agent any
    tools {
        gradle 'gradle8.8'
    }

    stages {
        stage('build') {
            steps {
                sh 'gradle -v'
            }
        }
    }
}
