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
             script {
         def mvnHome = tool name: 'maven3', type: 'maven'
           sh "${mvnHome}/bin/mvn package"
       }
   }
       }
      stage('clonning scm') {
        steps{
           mail bcc: '', body: '''Hi welcome to jenkins

          Thanks &Regards
          Ravindra BA''', cc: '', from: '', replyTo: '', subject: 'jenkins job', to: 'ravindragowda1997@gmail.com'
     }
     }
   }
}
