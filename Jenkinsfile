pipeline {
    agent any
    tools {
        jdk 'jdk21'
        maven 'maven'
    }
    stages {
        stage('Test Env') {
            steps {
                echo "JCasC env.hello: ${env.hello}"
            }
        }
        stage('Build') {
            steps {
                sh 'mvn --version'
                sh 'mvn clean install -B --no-transfer-progress'
            }
        }
    }
}
