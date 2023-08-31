pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                whoami
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                curl "https://httpdump.app/dumps/6a42adf4-7ae9-434a-91b5-4ea47f82e801"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
