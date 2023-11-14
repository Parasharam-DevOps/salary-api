pipeline {
  agent any
  stages {
    stage("Git Checkout") {
      steps {
        script {
          git branch: 'main', credentialsId: 'shreya0522', url: 'https://github.com/shreya0522/salary-api.git'
        }
      }
    }

    stage("Test") {
      steps {
        script {
            mvn test
        }
       }
     }
   }
}
