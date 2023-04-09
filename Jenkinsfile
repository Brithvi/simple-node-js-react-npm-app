pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello Build "'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Hello Test '
            }
        }
        stage('Deliver') {
            steps {
                sh 'echo "Hello Deliver '
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
            }
        }
     }
    }
}
