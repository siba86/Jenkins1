{
pipeline {
    agent any 

    stages {
        stage('Build and Test') {
            matrix {
                axes {
                    axis {
                        name 'PLATFORM'
                        values 'linux', 'macos', 'windows'
                    }
                    axis {
                        name 'BROWSER'
                        values 'firefox', 'chrome', 'safari'
                    }
                }
                stages {
                    stage('Build') {
                        steps {
                            echo "Construire pour ${PLATFORM} - ${BROWSER}"
                        }
                    }
                    stage('Test') {
                        steps {
                            echo "Tester pour ${PLATFORM} - ${BROWSER}"
                        }
                    }
                }
            }
        }

        stage('Deployment to Production') {
            steps {
                echo 'Déploiement en production !'
            }
        }
    }
}
}
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
