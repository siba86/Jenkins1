pipeline {
        stages('build') {
            failFast true 
            parallel {
                stage('build frontend') {
                    steps {
                        echo 'build frontend'
                    }
                }

                stage('build backend') {
                    steps {
                        echo 'build backend'
                    }
                }
            }
    }

    stage('deployment production') {
        steps {
            echo 'deploy'
        }
    }
}