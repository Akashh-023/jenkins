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
                // Create a directory and copy the latest code
                script {
                    sh 'mkdir -p /home/ec2-user/dest'
                    sh 'cp -r * /home/ec2-user/dest/'
                }
            }
        }
    }
}
