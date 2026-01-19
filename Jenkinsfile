pipeline{
  agent any 
  stages{
    stage("stage1- hello"){
      steps{
        echo "Hello from jenkins to the user testing auto trigger"
        echo "checking through ngrok"
      }
    }
    stage("stage2 - systeminfo"){
      steps{
        sh 'date'
        sh 'whoami'
        sh 'hostname'
      }
    }
  }
}
