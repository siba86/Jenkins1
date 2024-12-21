
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Commandes pour construire l'application, par exemple avec Maven
                sh 'mvn clean package'
            }
        }

        stage('Archive Artifacts') {
            steps {
                // Archivage des fichiers .jar ou .war générés dans le dossier 'target'
                archiveArtifacts artifacts: 'target/*.jar', allowEmptyArchive: true
            }
        }
    }
}
