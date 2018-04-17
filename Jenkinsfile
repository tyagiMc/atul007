pipeline{
agent{
  label "windows"
  }
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
  bat 'cd NumberGenerator $ mvn install'
  }
  post{
  success{
       junit 'NumberGenerator/target/surefire-reports/*.xml'
       }
       }
       
       }
       }
       }
  
  
  
  
  

