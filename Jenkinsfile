pipeline{
    agent any 
    environment {
        MY_VAR = 'une variable'
        MY_NUMBER = 123
    }

    stages {
        stage('buil') {
            steps {
               sh 'npm -v'
            }
        }
    }
}
