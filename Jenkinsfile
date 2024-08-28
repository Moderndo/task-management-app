pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                bat 'npm install'  // Installs dependencies
                bat 'npm run build'  // Runs the build script
            }
        }
        
        stage('Test') {
            steps {
                bat 'npm test'  // Runs the test script
            }
        }
        
        stage('Code Quality Analysis') {
            steps {
                bat 'npm run quality'  // Runs the code quality analysis script
            }
        }
        
        stage('Deploy') {
            steps {
                bat 'npm run deploy'  // Runs the deploy script
            }
        }
    }
}
