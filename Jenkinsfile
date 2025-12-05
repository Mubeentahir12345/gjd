pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello Jenkins!'
            }
        }
        stage('JCasC Env') {
            steps {
                echo "JCasC env.hello: ${env.hello}"
            }
        }
    }
}
