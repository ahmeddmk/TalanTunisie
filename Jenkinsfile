pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git {
                    url 'https://github.com/ahmeddmk/TalanTunisie.git'
                    credentialsId 'ahmed'
                }
            }
        }
        stage('Build') {
            steps {
                // Insert your build steps here
            }
        }
        stage('Test') {
            steps {
                // Insert your test steps here
            }
        }
        stage('Deploy') {
            steps {
                // Insert your deploy steps here
            }
        }
        stage('Create Pull Request') {
            steps {
                ghprbPullRequest(targetBranch: 'Development', title: 'My pull request', description: 'Please review my changes')
            }
        }
    }
}
