pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o hello hello.c'
            }
        }

        stage('Test') {
            steps {
                sh './hello'
            }
        }

        stage('Deploy') {
            steps {
              echo'Successfully Delpoyed'
            }
        }
    }

    post {
        failure{  
                    echo 'pipeline failed'
                }
            }
       

