pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from Git repository
                git 'https://your-repo-url.git'
            }
        }
        
        stage('Build') {
            steps {
                // Simulating a build step for an HTML project (usually no build in HTML, but could be for preprocessing)
                echo 'Building HTML project...'
            }
        }
        
        stage('Test') {
            steps {
                // Here, we could simulate running a test (like checking if the HTML file is valid)
                echo 'Running tests...'
                sh 'echo "Test passed!"'  // This is just a simulation
            }
        }
        
        stage('Deploy') {
            steps {
                // Simulating deployment of the HTML project (e.g., copying files to a server)
                echo 'Deploying HTML project...'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
