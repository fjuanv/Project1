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
    slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'bad', message: 'Assignment 4 - built', tokenCredentialId: 'cicdslak1', username: 'francisco.juan.v@gmail.com'
}
