pipeline {
    agent any


parameters {
    string(name: 'NAME', defaultValue: 'M. Jenkins', description: 'Qui est ce ?')
    text(name: 'TEXT', defaultValue: 'un text', description: 'Une description')
    booleanParam(name: 'TOGGLE', defaultValue: true, description: 'true ou false')
    choice(name: 'CHOICE', choices: ['un', 'deux', 'trois'], description: 'true ou false')
    password(name: 'PASSWORD', description: 'un mot de passe')
}
    stages {
        stage('build') {
            steps {
                echo "NAME : ${ NAME }"
                echo "NAME : ${ TEXT }"
                echo "NAME : ${ TOGGLE }"
                echo "NAME : ${ CHOICE }"
                echo "NAME : ${ PASSWORD }"
            }
        }
    }
}