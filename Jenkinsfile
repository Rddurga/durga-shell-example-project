pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout your project from the repository
                git 'https://your-repository-url.git'
            }
        }
        
        stage('Compile') {
            steps {
                script {
                    // Compile the Java program
                    sh 'javac HelloWorld.java'
                }
            }
        }
        
        stage('Run') {
            steps {
                script {
                    // Run the Java program
                    sh 'java HelloWorld'
                }
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline executed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
