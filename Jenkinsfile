pipeline {
    agent any

    stages {
        stage('Fetch') {
            steps {
                echo 'Fetching from Repo'
                git 'https://github.com/ann77382/javaep.git'
            }
        }
         stage('Build') {
            steps {
                echo 'Building the Program'
                bat 'javac hello.java'
            }
        }
        stage('Execute') {
            steps {
                echo 'Executing'
                bat 'java hello'
            }
        }
    }
    post{
        success{
            echo 'Pipeline built Successfully'
        }
        failure{
            echo 'Pipeline Failed'
        }
    }
}
