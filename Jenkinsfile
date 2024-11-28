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

        stage ('deployment production') {
            input {
                message 'Voulez-vous deployer en production'
                ok 'deployer'
                submitter 'admin, devops'
                submitParameter 'USER_SUBMIT'
                parameters {
                    string(name: 'VERSION', defaultValue: 'latest', description: 'une version')
                }
            }
        
            steps {
                echo "user : ${ USER_SUBMIT }"
                echo "version : ${ VERSION }"
                echo 'deploy'
            }
        }
    }
}
