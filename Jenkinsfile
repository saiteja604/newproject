pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/saiteja604/newproject.git'
         }
      }
     /* stage('Compile') {
         steps {
            bat 'mvn compile'
         }
      }
	   stage('Test') {
         steps {
            bat 'mvn test'
         }
      }*/
	   stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/workspace/Sample_Pipeline/target/exampleProj-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
