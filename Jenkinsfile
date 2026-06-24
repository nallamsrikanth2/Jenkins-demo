pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        // Timeout counter starts BEFORE agent is allocated
        timeout(time: 1, unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {
                sh "echo This is Build"
            }
        }
        stage('Test') {
            steps {
                sh "echo This is Test"
                sh "sleep 2"
            }
        }
        stage('Deploy') {
            steps {
                sh "echo This is Deploy"
            }
        }
    }
}