pipeline {
    agent any 

    parameters {
        string(name: 'NAME', defaultValue: 'M. Jenkins', description: 'Qui est-ce ?')
        text(name: 'TEXT', defaultValue: 'Un texte', description: 'Une description')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'True ou False')
        choice(name: 'CHOICE', choices: ['un', 'deux', 'trois'], description: 'Liste de choix')
        password(name: 'TEXPASSWORDT', defaultValue: 'un mot de passe')
    }
    stages {
        stage('build') {
            steps {
                script {
                    echo "NAME: ${params.NAME}"
                    echo "TEXT: ${params.TEXT}"
                    echo "TOGGLE: ${params.TOGGLE}"
                    echo "CHOICE: ${params.CHOICE}"
                    echo "TEXPASSWORDT: ${params.TEXPASSWORDT}"
                }
            }
        }
    }
}
