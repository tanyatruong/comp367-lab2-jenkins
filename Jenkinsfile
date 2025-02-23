pipeline {
    agent any
    
    triggers {
        githubPush()
    }
    
    stages {
        stage('Display Information') {
            steps {
                echo "Jenkins URL: ${JENKINS_URL}"
                echo "Build ID: ${BUILD_ID}"
            }
        }
    }
}
