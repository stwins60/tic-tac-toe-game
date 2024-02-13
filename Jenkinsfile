pipeline {
    agent any

    tools {
        nodejs 'node21'
    }

    environment {
        DOCKERHUB_CREDENTIALS = credentials('d4506f04-b98c-47db-95ce-018ceac27ba6')
        SCANNER_HOME= tool 'sonar-scanner'
        IMAGE_NAME = 'idrisniyi94/tic-tac-toe-game'
        IMAGE_TAG= "${env.BUILD_NUMBER}"
    }

    stages {
        stage('Clean workspace') {
            steps {
                cleanWs()
            }
        }
}