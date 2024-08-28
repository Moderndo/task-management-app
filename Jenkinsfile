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

        // Additional stages can be added here
    }
}
