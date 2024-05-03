pipeline {
    agent any
    stages {
        stage('install npm') {
            steps {
                bat 'npm install'
            }
        }
        stage('install cypress') {
            steps {
                bat 'npm install cypress'
            }
        }
        stage('test') {
            steps {
                // Set environment variable NO_COLOR to 1 and run Cypress tests
                bat 'set NO_COLOR=1 && npx cypress run --browser chrome'
            }
        }
    }
}
