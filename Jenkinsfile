pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo "Test"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploy"
            }
        }
    }
}
def notifyBuild(String buildStatus = 'STARTED') {
    slackSend (channel: 'jenkins', color: 'bad', message: 'Assignment 4 - built', tokenCredentialId: 'cicdslak1')
}
