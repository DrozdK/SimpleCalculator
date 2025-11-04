pipeline {
    agent any
    tools {
        maven "M3"
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/DrozdK/SimpleCalculator.git'
            }
        }
        stage('Run tests') {
            steps {
                sh "mvn clean test"
            }
        }
    }
}