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
              sh ' wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash'
            }
        }
         stage('nvm') {
            steps {
              sh 'source ~/.profile'
            }
        }
         stage('nvm2') {
            steps {
              sh 'nvm install node'
            }
        }
    }
}
