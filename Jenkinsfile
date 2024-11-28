pipeline{
    agent {
        docker {
            image 'node:21-alpine'
        }

    }
    options {
        timeout(time: 1, unit: "HOURS")
    }

    stages {
        stage('buil') {
            options {
                timestamps()
            }
            steps {
               sh 'npm -v'
            }
        }
    }
    post {
        always {
            echo 'always !'

        }
        success {
            echo 'success !'
        }

    }

    
}
