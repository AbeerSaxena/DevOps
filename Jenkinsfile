pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your/repo.git'
            }
        }
        stage('Compile and Test') {
            steps {
                sh 'mvn clean compile test'
            }
        }
        stage('Package as War') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
