pipeline{
    agent any 
    docker {
        image 'node:21-alpine'
    }

    stages {
        stage('buil') {
            steps {
               sh 'npm -v'
            }
        }
    }
}
