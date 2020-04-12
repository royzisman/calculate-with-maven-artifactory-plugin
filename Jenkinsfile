pipeline {
  agent any
  tools {
    maven 'Maven 3.3.9'
    jdk 'jdk8'
  }
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/royzisman/calculate-with-maven-artifactory-plugin.git'
      }
    }
    stage('Build and Deploy') {
       steps {
         sh 'mvn clean deploy -Dusername=admin -Dpassword=AP974LdvTpjLKmhcm6r9cng68FJ -Dbuildnumber=7 -s settings.xml'
       }
    }
}
}











