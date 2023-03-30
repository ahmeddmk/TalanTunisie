pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git {url 'https://github.com/ahmeddmk/TalanTunisie.git'
                     credentialsId 'push'
                }
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Hello, World!"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Hello, World!"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Hello, World!"'
            }
        }
        stage('Create Pull Request') {
            steps {
                ghprbPullRequest(targetBranch: 'Development', title: 'My pull request', description: 'Please review my changes')
            }
        }
    }
}
