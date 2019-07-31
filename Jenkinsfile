node {
   
   stage('Code Checkout') { 
      git credentialsId: 'github', url: 'https://github.com/techproject123/maven_apps.git'
    }
   stage('Build') {
    withMaven(jdk: 'jdk', maven: 'maven') {
     sh 'mvn clean compile'
      }
    }
   stage('Unit Test run') {
   withMaven(jdk: 'jdk', maven: 'maven'){
     sh 'mvn test'
      } 
    }
   stage('Packageto Jfrog') {
    withMaven(jdk: 'jdk', maven: 'maven') {

     sh 'mvn package'
      }
    }
   stage('Deploy to Dev') {
     
    }
   stage('Automation Testing') {
     
    }
   stage('Deploy to Test') {
     
    }
   stage('Smoke Testing') {
     
    }
   stage('Deploy to Prod') {
     
    }
   stage('Acceptance Testing') {
     
    }
}
