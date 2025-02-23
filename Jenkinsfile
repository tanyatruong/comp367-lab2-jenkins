pipeline {
    agent any

    stages {
        stage('Print Webhook Data') {
            steps {
                script {
                    echo "Jenkins URL: ${JENKINS_URL}"
                    echo "Build ID: ${BUILD_ID}"
                }
            }
        }
    }
}
