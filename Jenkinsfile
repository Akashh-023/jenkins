pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the develop branch
                git branch: 'develop', url:  'https://github.com/Akashh-023/jenkins.git'
            }
        }
        stage('Pull Code') {
            steps {
                // Create a directory and pull the latest code
                script {
                    bat 'mkdir \\home\\ec2-user\\dest'
                    bat 'xcopy * \\home\\ec2-user\\dest /s /e /y'
                }
            }
        }
    }
}
