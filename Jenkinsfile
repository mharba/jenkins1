pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build'
            }
        }
    }
    stages {
        stage('deployment production') {
            input {
                message 'Voulez-vous deployer en production ?'
                ok 'Deployer !'
                submitter 'admin,devops'
                submitParameter 'USER_SUBMIT'
                parameters {
                   string(name: 'VERSION', defaultValue: 'latest', description: 'Une version') 
                }
            }
            steps {
                echo "user: ${ USER_SUBMIT }"
                echo "version: ${ VERSION }"
                echo 'deploy !'
            }
        }
    }
}