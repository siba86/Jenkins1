pipeline{
    agent any 

    stages {
        stage('buil') {
            steps {
                echo "BRANCH_NAME : ${env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY : ${env.BRANCH_IS_PRIMARY}"
                echo "CI : ${env.CI}"
                echo "BUILD_NUMBER : ${env.BUILD_NUMBER}"
                echo "JENKINS_URL : ${env.JENKINS_URL}"
            }
        }
    }
}
