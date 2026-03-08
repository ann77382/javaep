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
                echo "Building Java Project"
                bat 'javac hello.java'
                bat 'java hello'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }

    }
}
