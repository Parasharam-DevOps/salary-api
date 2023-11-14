pipeline {
  agent any
  stages {
    stage("Git Checkout") {
      steps {
        script {
          git branch: 'main', credentialsId: 'shreya0522', url: 'https://github.com/shreya0522/aws-terraform-final.git'
        }
      }
    }
