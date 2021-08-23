pipeline 
 {
  agent any
  stages{
   stage('Build'){
   steps{
   bat 'mvn clean install'
   }
   }
  
   stage('Unit Testing'){
   steps{
   bat 'mvn clean package'
   }
   }
  
   stage('Deploy Application'){
   steps{
   bat 'mvn package deploy -DmuleDeploy'
  }
  }
  }
 }