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
              sh 'sudo yum install nodejs -y'
            }
        }
        stage('npm') {
            steps {
              sh 'nvm install node'
            }
        }
        // stage('npm') {
        //     steps {
        //       sh  'cd node-js-web-application'
        //     }
        // }
    }
}
