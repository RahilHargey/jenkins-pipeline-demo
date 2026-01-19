pipeline{
  agent any 
  stages{
    stage("stage1- hello"){
      steps{
        echo "Hello from jenkins to the user"
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
