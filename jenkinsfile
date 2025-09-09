pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', credentialsId: '61cbc151-9fc5-45a0-84e3-6653a99355e2', url: 'https://github.com/samruddhi0619/TEIT31.git'
            }
        }
         stage('compile') {
            steps {
                bat 'javac HelloJava.java'
            }
        }
         stage('run') {
            steps {
                bat 'java HelloJava'
            }
        }
    }
}
