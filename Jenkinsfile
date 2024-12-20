
pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh 'echo hello > world.txt' // Crée un fichier texte avec "hello" comme contenu
                archiveArtifacts artifacts: '*.txt' // Archive les fichiers texte créés
            }
        }
    }
}
