pipeline{

  agent any 

  stages{

    stage('Test Connetivity'){

      steps{
        sshagent(credentials: ['ssh-server'] ){
          sh '''
              ssh -o StrictHostKeyChecking=no ubuntu@43.205.238.10 hostname
            '''
        }
      }
    }
  }
}
