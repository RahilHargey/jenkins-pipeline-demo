pipeline {
    agent any

    stages {
        stage('Test SSH Connection') {
            steps {
                sshagent(credentials: ['ssh-server']) {
                    sh """
                        ssh -o StrictHostKeyChecking=no ubuntu@3.109.184.15 hostname
                        ssh -o StrictHostKeyChecking=no ubuntu@3.109.184.15 whoami
                        echo "ssh Done successfully"
                    """
                }
            }
        }
    }
}
