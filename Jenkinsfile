pipeline {
   stages {
     stage('clonning scm') {
       git 'https://github.com/ravindrabadevops/warfile.git'
     }
       stage('Build') {
       sh 'mvn package'
       }
   }
}
