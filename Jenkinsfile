pipeline {
    agent any
    parameters{
        choice(name: 'DEPLOY_TO', choices: ['PreProd', 'production'], description: 'Production ?')
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
                    equals expected: 'production', actual: params.DEPLOY_TO
                }
            }
            steps {
                echo 'deploy !'
            }
        }
    }
}
