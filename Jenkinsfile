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
  bat 'start C:\Users\Administrator\Downloads\apache-tomcat-8.5.30-windows-x64\apache-tomcat-8.5.30\bin\startup.bat'
  }
  post{
  success{
       junit 'NumberGenerator/target/surefire-reports/*.xml'
       }
       }
       
       }
       }
       }
  
  
  
  
  

