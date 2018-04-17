pipeline{
  agent any
  stages{
    stage('push artifacts')
    {
      steps
      {
        bat 'mkdir archive'
        bat 'echo test  > archive/test.txt'
        zip zipFile: 'test.zip' , archive: false, dir: 'archive'
        archiveArtifacts artifacts: 'test.zip', fingerprint: true
      }
    }
    }
  }
  
  
  
  
  

