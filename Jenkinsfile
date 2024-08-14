pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the develop branch
                git branch: 'develop', url: 'https://github.com/Akashh-023/jenkins.git'
            }
        }
        stage('Pull Code') {
            steps {
                // Create a directory and pull the latest code
                script {
                    sh 'mkdir -p /C:\Users\ASA960\Documents\code'
                    sh 'cp -r * /C:\Users\ASA960\Documents\code/'
                }
            }
        }
    }
}
