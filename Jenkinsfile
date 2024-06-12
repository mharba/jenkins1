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
                branch 'main'
            }
            steps {
                echo 'deploy !'
            }
        }
    }
<<<<<<< HEAD
    
}
=======
}
>>>>>>> cdc73a7 (change)
