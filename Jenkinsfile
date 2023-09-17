pipeline {
   stages {
     stage('clonning scm') {
        steps{
       git 'https://github.com/ravindrabadevops/warfile.git'
     }
     }
       stage('Build') {
          steps {
       sh 'mvn package'
       }
   }
   }
}
