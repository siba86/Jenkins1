pipeline {
    agent any 

    parameters {
        string(name: 'NAME', defautValue: 'M. Jenkins', description: 'Qui estr ce ?')
        text(name: 'TEXT', defautValue: 'un text', description: 'une description')
        booleanParam(name: 'TOGGLE', defautValue: true, description: 'true ou false')
        choice(name: 'CHOICE', defautValue: ['un', 'deux', 'trois'], description: 'liste')
        password(name: 'TEXPASSWORDT', defautValue: 'un mot de passe')
    }
    stages {
        stage ('build') {
            steps {
                echo "NAME: ${NAME }"
                echo "TEXT: ${TEXT }"
                echo "TOGGLE: ${TOGGLE }"
                echo "CHOICE: ${CHOICE }"
                echo "TEXPASSWORDT: ${TEXPASSWORDT }"
            }
        }
    }
}