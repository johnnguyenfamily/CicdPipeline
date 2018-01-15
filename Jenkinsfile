#!groovy

node {

    stage('checkout') {
      checkout scm
    }
    
    stage('build') {
      sh "mvn clean install -Dmaven.test.skip=true"
    }
    
    stage('test') {
      sh "mvn test"
    }
    
}    
