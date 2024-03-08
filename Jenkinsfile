pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    // Compile the .cpp file using shell script
                    sh 'g++ -o output_file hello1.cpp'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    // Print output of .cpp file using shell script
                    sh './output_file'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                // Add deployment steps if applicable
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
