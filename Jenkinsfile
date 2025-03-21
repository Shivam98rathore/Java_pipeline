// pipeline {
    environment {
        Version = "3.6"
    }
    agent any
    stages {
        stage("Compile") {
            steps {
                bat 'javac Test.java'
                bat 'echo %Version%'
                // bat 'echo "${env.Version}"' not working 
            }
        }
        stage("run java program") {
            steps {
                bat 'java Test'
            }
        }
    }
    post {
        always {
            bat 'echo "this is always"'
        }
        success {
            bat 'echo "this is a success"'
        }
        failure {
            bat 'echo "this is a failure"'
        }
    }
}
