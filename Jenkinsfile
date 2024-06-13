pipeline {
    agent any

    stages {
        stage('build and test') {
            matrix {
                axes {
                    axis {
                        name 'PLATEFORM'
                        values ' linux', 'macos', 'windows'
                    }
                    axis {
                        name 'BROWSER'
                        values ' firefox', 'chrome', 'safari'
                    }
                }
                stages {
                    stage('build') {
                        steps {
                            echo "Construire pour ${ PLATEFORM } - ${ BROWSER }"
                        }
                    }
                    stage('test') {
                        steps {
                            echo "test pour ${ PLATEFORM } - ${ BROWSER }"
                        }
                    }
                }
            }
        }
        stage('deployment production') {
            steps {
                echo 'Deploy !'
            }
        }
    }
}
