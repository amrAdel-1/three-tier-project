pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'nodejs-app', url: 'https://github.com/amrAdel-1/three-tier-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t nodejs-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 --name nodejs nodejs-app'
            }
        }
    }
}
