pipeline {
    agent any

    environment {
        JENKINS_URL = "${env.JENKINS_URL}"
        BUILD_ID = "${env.BUILD_ID}"
    }

    stages {
        stage('Print Webhook Data') {
            steps {
                script {
                    // Print Jenkins Environment Variables
                    echo "Jenkins URL: ${JENKINS_URL}"
                    echo "Build ID: ${BUILD_ID}"

                    // Check if GitHub webhook sent additional data
                    if (env.GIT_COMMIT) {
                        echo "Git Commit SHA: ${env.GIT_COMMIT}"
                    }
                    if (env.GIT_BRANCH) {
                        echo "Git Branch: ${env.GIT_BRANCH}"
                    }
                }
            }
        }
    }
}
