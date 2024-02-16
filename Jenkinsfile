pipeline {
  agent any

  tools {nodejs "node"}

  stages {    
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Hamzaselmi99/Quiz.git'
      }
    }        
    stage('Install dependencies') {
      steps {
        sh 'npm i -save express'
      }
    }     
    stage('Test') {
      steps {
         sh 'node Server.js'
      }
    }             
  }
}
