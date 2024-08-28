pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                bat 'echo "Building the project..."'
                bat 'npm install'
                bat 'npm run build'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test' 
            }
        }

        stage('Code Quality Analysis') {
            steps {
                bat 'npm run lint' // This will run ESLint to check for code quality issues
            }
        }

        // Deploy, Release, and Monitoring stages can be added here if needed
    }
}
