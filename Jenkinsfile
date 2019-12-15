node
{
 stage('source code management')
  {
    git 'https://github.com/spring-projects/spring-petclinic.git'
  }
 stage('build the package')
  {
    sh label: '', script: 'mvn package'
  }
 stage('archival')
  {
    archive 'target/*.jar'
  }

 stage('test results')
  { 
    junit 'surefire-reports/*.xml'
  } 
    
    

