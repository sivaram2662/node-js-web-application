pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
              git branch: 'main', url: 'git@github.com:sivaram2662/node-js-web-application.git'
            }
        }
        stage('node') {
            steps {
              sh 'sudo yum install node -y'
            }
        }
    }
}
