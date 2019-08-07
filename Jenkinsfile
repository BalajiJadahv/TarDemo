pipeline{
agent any

stages{
    stage('Checkout Code') {
          steps{  
               git 'https://github.com/BalajiJadahv/soccer-stats.git'
               }
           }
    stage('Build Stage'){
             steps{
       
                  sh 'mvn clean assembly:assembly'
             }   
       }
  }
} 

