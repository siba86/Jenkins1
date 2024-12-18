pipeline {
    agent any 

    stages {
        stage('build') {
            steps {
                echo 'build'
            }
        }

        stage ('deployment production') {
            when {
                branch 'main'
            }
        
            steps {
                echo 'deploy'
            }
        }
    }
}
