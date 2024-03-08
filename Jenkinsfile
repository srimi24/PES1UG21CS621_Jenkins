pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                    build 'PES1UG21CS621-1'
                    sh 'g++ main/hello.cpp -o output'
            }
        }
        
        stage('Test') {
            steps {
                    sh './outp'
            }
        }
        
        stage('Deploy') {
            steps {
                  echo "deploy"
            }
        }
      }
      post{
          failure{
            error 'pipeline failed'
          }
    }
}
