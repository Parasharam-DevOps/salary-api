
pipeline {
    agent any

    tools {
       maven 'maven'
    }

    stages {
        stage("Git Checkout") {
            steps {
                script {
                    git branch: 'main', url: 'https://github.com/shreya0522/salary-api.git'
                }
            }
        }

        stage("Bug Analysis ") {
            steps {
               script {
                 sh 'mvn compile'
                 sh 'mvn spotbugs:spotbugs'
                 sh 'mvn site'
               }
            }
        }

      }
    }

