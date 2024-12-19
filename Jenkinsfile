pipeline {
        agent any 

        stages {
            stage('build and test') {
                matrix {
                    axes {
                        axis {
                        name 'PLATEFORM'
                        values 'linux', 'macos', 'windows'
                    }
                    axis {
                        name 'BROWSER'
                        values 'firefox', 'chrome', 'safari'
                    }
                }
                stages {
                    stage('build') {
                        echo "construire pour ${PLATEFORM} - ${BROWSER}"
                    }
                }
                stages {
                    stage('test') {
                        echo "construire pour ${PLATEFORM} - ${BROWSER}"
                    }
                }
            }
        }

        stage('deployement production') {
            steps {
                echo 'deploy !'
            }
        }
    }
}
