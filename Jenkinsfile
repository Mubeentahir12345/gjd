pipeline {
    agent any
    tools {
        jdk 'jdk21'
        maven 'maven'
    }
    environment {
        hello = "Hello from Jenkinsfile Runner!"
    }
    stages {
        stage('Test Env') {
            steps {
                echo "${env.hello}"
            }
        }
        stage('Build') {
            steps {
                sh 'mvn --version'
                sh 'mvn clean install'
            }
        }
    }
}
