pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // For Windows: Replace 'sh' with 'bat'
                bat 'echo "Building the project..."'
                bat 'npm install'
                bat 'npm run build'
            }
        }

        // Additional stages can be added here
    }
}
