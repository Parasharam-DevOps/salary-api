      pipeline {
                agent any
                tools {
                    maven "mvn"
                }
                stages {
                    stage('Checkout') {
                        steps {
                            git branch: 'main', url: 'https://github.com/Parasharam-DevOps/salary-api.git'
                        }
                    }
                    stage('Test') {
                        steps {
                            echo "Executing Java Unit Testing"
                            sh 'mvn test'
                        }
                    }
                }
            }
