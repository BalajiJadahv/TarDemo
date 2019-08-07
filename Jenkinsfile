pipeline{
agent any

stages{
    stage('Checkout Code') {
          steps{  
               git 'https://github.com/BalajiJadahv/TarDemo.git'
               }
           }
    stage('Build Stage'){
             steps{
       
                  sh 'mvn clean assembly:single'
                  stash name: "artifact", includes: "target/**.tar"
  //                echo "Artifact stored is " $artifact
             }   
       }
  }
} 

