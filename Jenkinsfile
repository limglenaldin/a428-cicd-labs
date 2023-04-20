pipeline {
    agent {
        docker {
            image 'node:16-buster-slim' 
            args '-p 3000:3000'
            args '---dns 8.8.8.8'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}