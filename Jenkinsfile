pipeline {
   agent any
   stages {
     stage('clonning scm') {
        steps{
       git 'https://github.com/ravindrabadevops/warfile.git'
     }
     }
       stage('Build') {
          steps { 
           def mvnHome = tool name: 'maven3', type: 'maven'
           sh "${mvnHome}/bin/mvn package"
       }
   }
   }
}
