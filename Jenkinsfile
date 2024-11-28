pipeline {
    agent any 

    triggers {
        cron('* * * * *')
    }

    stages {
        stage('build') {
            steps {
                echo 'build'
            }
        }
    }
}
