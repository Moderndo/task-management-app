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
                bat 'npm run lint' // This runs ESLint to check the code quality
            }
        }

        // You can add Deploy and other stages if needed
    }
}
