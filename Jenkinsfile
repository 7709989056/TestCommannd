pipeline {
  agent none
  options { 
      skipDefaultCheckout() 
  }
  stages{
    stage('SCM operation'){
      agent {label 'SlaveSCMConnected'}
      steps{
        checkout scm
        sh 'mvn clean install'
      }
   }
