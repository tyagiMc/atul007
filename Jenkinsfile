pipeline{
agent any
  tools{
  maven 'maven3.5.3'
  jdk 'java8'
  }
  stages{
  stage('Initialize'){
  steps{
  bat '''
  echo "PATH = $PATH$"
  echo "M2_HOME = $M2_HOME"
  '''
  }
  }
  stage('Build')
  {
  steps
  {
  bat 'cd target'
  }
  post{
  success{
       junit 'NumberGenerator/target/surefire-reports/*.xml'
       }
       }
       
       }
       }
       }
  
  
  
  
  

