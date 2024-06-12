pipeline {
    agent any
    parameters{
        choice(name: 'DEPLOY_TO', ['production', 'PreProd'], defaultValue: "Preprod", description: 'Production ?')
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
