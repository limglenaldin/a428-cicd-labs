pipeline {
    agent {
        docker {
            image 'node:18-buster-slim' 
            args '-p 3000:3000'
            args '--network host'
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