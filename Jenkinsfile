pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo Build test'
            }
        }
        stage('test') {
            steps {
                sh 'python helloworld.py'
            }
        }
    }
}