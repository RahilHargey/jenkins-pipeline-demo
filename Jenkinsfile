pipeline {
    agent any

    stages {
        stage('Test SSH Connection') {
            steps {
                sshagent(credentials: ['ssh-server']) {
                    sh """
                        ssh -o StrictHostKeyChecking=no ubuntu@43.205.238.10 hostname
                        ssh -o StrictHostKeyChecking=no ubuntu@43.205.238.10 whoami
                        echo "ssh Done successfully"
                    """
                }
            }
        }
    }
}
