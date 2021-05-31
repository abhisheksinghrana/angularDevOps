pipeline {
    agent any
    tools {
        nodejs 'NodeJS'
    }
    stages {
        stage('Installing NPM dependencies') {
            steps {
                echo 'Installing packages...'
                sh 'npm install'
            }
        }

        stage('Run Lint') {
            steps {
                echo 'Linting...'
                sh 'npm run lint'
            }
        }

        stage('Run Unit Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm run build'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}