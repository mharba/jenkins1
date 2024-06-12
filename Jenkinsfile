pipeline {
    agent any
    parameters{
        booleanParam(name: 'DEPLOY_TO', default: false, description: 'Production ?')
    }

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
                    equals expected: true, actual: params.DEPLOY_TO
                }
            }
            steps {
                echo 'deploy !'
            }
        }
    }
}
